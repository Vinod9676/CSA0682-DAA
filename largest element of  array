#include <stdio.h>
void main() {
    int arr[100], max, size, i;
    printf("Enter the size of the array: ");
    scanf("%d", &size);
    printf("Enter %d elements in the array: ", size);
    for(i=0; i<size; i++) {
        scanf("%d", &arr[i]);
    }
    max = arr[0];
    for(i=1; i<size; i++) {
        if(max < arr[i]) {
            max = arr[i];
        }
    }
    printf("Largest element of the array is %d", max);
}
