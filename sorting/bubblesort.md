# Bubble Sort 

![alt text](/images/bubblesort.png)

```
function bubbleSort(items) {
    var length = items.length;
    //Number of passes
    for (var i = 0; i < length; i++) { 
        //Notice that j < (length - i)
        for (var j = 0; j < (length - i - 1); j++) { 
            //Compare the adjacent positions
            if(items[j] > items[j+1]) {
                //Swap the numbers
                var tmp = items[j];  //Temporary variable to hold the current number
                items[j] = items[j+1]; //Replace current number with adjacent number
                items[j+1] = tmp; //Replace adjacent number with current number
            }
        }        
    }
}

```



* The complexity of bubble sort is O(n2)  in both worst and average cases, because the entire array needs to be iterated for every element.
