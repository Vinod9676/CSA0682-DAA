#include <stdio.h>
int main() {
    int m, n, p, q, i, j, k;
    printf("Enter rows and columns of first matrix: ");
    scanf("%d %d", &m, &n);
    int first[m][n];
    printf("Enter elements of first matrix:\n");
    for (i = 0; i < m; ++i) {
        for (j = 0; j < n; ++j) {
            scanf("%d", &first[i][j]);
        }
    }
    printf("Enter rows and columns of second matrix: ");
    scanf("%d %d", &p, &q);
    if (n != p) {
        printf("Matrices cannot be multiplied!");
        return 0;
    }
    int second[p][q], multiply[m][q];
    printf("Enter elements of second matrix:\n");
    for (i = 0; i < p; ++i) {
        for (j = 0; j < q; ++j) {
            scanf("%d", &second[i][j]);
        }
    }
    for (i = 0; i < m; ++i) {
        for (j = 0; j < q; ++j) {
            multiply[i][j] = 0;
        }
    }
    for (i = 0; i < m; ++i) {
        for (j = 0; j < q; ++j) {
            for (k = 0; k < n; ++k) {
                multiply[i][j] += first[i][k] * second[k][j];
            }
        }
    }
    printf("Product of the matrices:\n");
    for (i = 0; i < m; ++i) {
        for (j = 0; j < q; ++j) {
            printf("%d ", multiply[i][j]);
            if (j == q - 1)
                printf("\n");
        }
    }
    return 0;
}
