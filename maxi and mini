#include <stdio.h>
#include <stdlib.h>
#include <limits.h>

struct Pair {
    int min, max;
};


struct Pair findMinAndMax(int arr[], int low, int high)
{
    struct Pair result, left, right;


    if (low == high) {
        result.max = arr[low];
        result.min = arr[low];
        return result;
    }


    if (high - low == 1) {
        if (arr[low] < arr[high]) {
            result.max = arr[high];
            result.min = arr[low];
        }
        else {
            result.max = arr[low];
            result.min = arr[high];
        }
        return result;
    }

   
    int mid = (low + high) / 2;

    
    left = findMinAndMax(arr, low, mid);

    
    right = findMinAndMax(arr, mid + 1, high);

    
    result.max = (left.max > right.max) ? left.max : right.max;

    
    result.min = (left.min < right.min) ? left.min : right.min;

    return result;
}

int main(void)
{
    int arr[] = { 7, 2, 9, 3, 1, 6, 7, 8, 4 };
    int n = sizeof(arr) / sizeof(arr[0]);

    struct Pair result = findMinAndMax(arr, 0, n - 1);

    printf("The minimum element in the array is %d\n", result.min);
    printf("The maximum element in the array is %d\n", result.max);

    return 0;
}
