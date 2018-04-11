
### Question Three

Write a declaration for an array that will hold 50 type long values
``` 
	long A[50] = 0
```
Show a statement that assigns the value of 123.456 to the 50th element in the array from the above question
``` 
A[49] = 123.456
```

What is the values of x when the following statement in complete ?
```
  for (x = 0; x < 100; x++)
```
The Value of x is
``` 
100
```
What is the value of ctr when the following statement is compelte

```
for(ctr = 2; ctr < 10; ctr += 3)
```
The Value of ctr is
``` 
11
```

Write a while statement to count from 1 to 100 by 3s
```c
int x = 1;
while(x<=100){
	printf("%d",x);	
	x++;
}
```

What is wrong with the following code fragment (MAXVALUES is not the problem !)

``` 
for (counter = 1; counter < MAXVALUES; counter++ );
printf("\nCounter = %d", counter);
```
>The problem is with the counter variable in the printf statement. the variable is not defined 
>

Write a function named addarrays() that accepts two arrays that are the same size. The function should add each element in the arrays together and place the values in a third array.

```

double addarrays(int *array1, int *array2){
	if(sizeof(array1) != sizeof(array2)){
		printf("ARRAYS NOT THE SAME SIZE");
		return 0;
	}else{
	    int x = sizeof(array1);
		double newArray[x];
		int z = 0;
		for(int i =0;i<x;i++){
			z = array1[i]+array2[i];
			newArray[i] = z;
		}
        return 1;
	}
}

```

Modify the function you created to return a pointer to the array containing the totals. Place this function in a program that also displays the values in all three arrays.

```
#include <stdio.h>
int newArray[];
int * addarrays(int *array1, int *array2){
	if(sizeof(array1) != sizeof(array2)){
		printf("ARRAYS NOT THE SAME SIZE");
		return 0;
	}else{
	    int x = sizeof(array1);
		newArray[x];
		int z = 0;
		for(int i =0;i<=x;i++){
			z = array1[i]+array2[i];
			newArray[i] = z;
		}
       return newArray;
	}
}

int main(){
    int A[5] = {10,20,30,40,500}, B[5] = {10,9,8,7,6};       
    int *C = addarrays(A,B);
	printf("FIRST ARRAY \n");
	for(int i =0;i<5;++i){
	   printf("%d, ",A[i]);
	}
	printf("\n");

	printf("SECOND ARRAY \n");
	for(int i =0;i<5;++i){
	   printf("%d, ",B[i]);
	}
	printf("\n");

	printf("THIRD ARRAY\n");
	for(int i=0;i<=sizeof(*C);i++){
	   printf("%d, ",C[i]);
	}
	printf("\n");
    
}
		
```
