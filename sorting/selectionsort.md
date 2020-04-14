# Selection Sort 

![alt text](/images/selectionsort.png)

```
function selectionSort(arr) {
    var temp = 0;
    for (var i = 0; i < arr.length; ++i) {
        for (var j = i + 1; j < arr.length; ++j) {
            if (arr[i] > arr[j]) { // compare element with the reset of other element
                temp = arr[i];  // swap the valuse from smallest to gretest
                arr[i] = arr[j];
                arr[j] = temp;
            }
        }
    }
    return (arr);
}

selectionSort([4,6,5,3,7,9]);

```



* The complexity of selection sort is O(n2)  in both worst and average cases.


![alt text](/images/complexity.png)