# EX-NO-6-Pseudo-Random-Number

# AIM: 

Implementation of Pseudorandom Number Generation Using Standard library

# Algorithm:

1.Accept user input for the number of random numbers (count), minimum value (min), and maximum value (max).

2.Initialize the random seed using the current time (srand(time(NULL))).

3.Start a loop that runs count times to generate random numbers.

4.In each iteration, calculate a random number between min and max using the formula (rand() % (max - min + 1)) + min

5.Print the generated random number.

6.Repeat until count random numbers are generated, then terminate the program.

# Program:
```

#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() 
{
    int count, min, max;
    printf("Enter the number of random numbers to generate: ");
    scanf("%d", &count);
    printf("Enter the minimum value: ");
    
    scanf("%d", &min);
    printf("Enter the maximum value: ");
    scanf("%d", &max);
    srand(time(NULL));
    printf("Pseudorandom numbers:\n");   
    for (int i = 0; i < count; i++) 
    {
        int random_number = (rand() % (max - min + 1)) + min;
        printf("%d\n", random_number);
    }
    return 0;
}

```

# Output :
![image](https://github.com/user-attachments/assets/e19a99eb-9cd4-42e5-8566-13f48cd4b1d3)



# Result:
Thus the program to generate random numbers is implemented successfully






