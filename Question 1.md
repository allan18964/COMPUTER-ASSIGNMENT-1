----
###Question One
Fix the Bug in the following code so that it runs correctly
```c
	/* a program with problems... */
	#include <stdio.h>
	int x= 1:
	main()
	{
	if( x = 1);
	    printf(" x equals 1" );
	otherwise
	    printf(" x does not equal 1");
	return 0;
	}
```
Problems
1. colon instead of semi-colon after int x=1
2. use of otherwise instead of else
3. if(x=1) must be a condition not assignment. so corrected to if(x==1)

``` c
#include <stdio.h>
int x = 1;
int main(){
    if(x == 1){
	   printf(" x equals 1" );C
    }
    else{
	printf(" x does not equal 1");
    }
    return 0;
}
```
_____________
