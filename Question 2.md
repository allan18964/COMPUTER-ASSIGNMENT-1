____________________
### Question 2
Write a header for a function named do_it() that takes three type char arguments and returns a type float to the calling program.
	
	float do_it(char arg1, char arg2, char arg3);

Write a header for a function named print_a_number() that takes a single type int argument and doesn't return anything to the calling program.
```h
void print_a_number(int arg1);
```

What's wrong with the following program ?

```c
#include <stdio.h>
void print_msg( void );
main(){
    print_msg("This is a message to print");
    return 0;
}
void print_msq( void )
{
    puts("This is a message to print");
    return 0;
}
```
Answer

function print_msg is not defined. so i redefine **print_msq** as **print_msg**

the function print_msg takes no arguments. I redefine it so as to take a single  character pointer argument.

The function print_msg returns void. I removed the return statement.


```C
#include <stdio.h>
void print_msg( char *b);
main(){
    print_msg("This is a message to print");
    return 0;
}
void print_msg(char *arg)
{
    puts("This is a message to print");
}
```
