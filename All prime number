#include <stdio.h>
#include <math.h>

int is_prime(int n) {
  if (n <= 1) {
    return 0;
  }
  
  if (n == 2) {
    return 1;
  }
  
  if (n % 2 == 0) {
    return 0;
  }
  
  int limit = (int) sqrt(n);
  for (int i = 3; i <= limit; i += 2) {
    if (n % i == 0) {
      return 0;
    }
  }
 
  return 1;
}


void print_primes(int limit) {
  printf("The prime numbers up to %d are:\n", limit);
  for (int i = 2; i <= limit; i++) {
    if (is_prime(i)) {
      printf("%d ", i);
    }
  }
  printf("\n");
}


int main() {
 
  int limit;
  printf("Enter a positive integer as the limit: ");
  scanf("%d", &limit);
  
 
  print_primes(limit);
  
  return 0;
}
