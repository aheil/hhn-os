In this lab you will learn about the adresses of the process of a small program written in C. 

Actually, you will only see the virtual adresses where your process thinks it resides.  

The physical adresses of your process are known only by the operating system. In a later lecture we will investigate how the operating system (and the hardware) perform the address translation from virtual to phyiscal addresses.

The following programm will provide the virtual adresses of your memory segments of the process. 

```c
#include <stdio.h>
#include <stdlib.h>

int main(int argc, char *argv[])
{
    printf("Location of code : %p\n", main);
    printf("location of heap : %p\n", malloc(100e6));
    
    int x = 3;
    printf("location of stack: %p\n", &x);
    return x;
}
```


**Tasks**
* Compile and start the program 
* Try to answer the following questions 
    * Why do we need to call the *malloc*-funciton to obtain tzhe heap address?
    * Why do we need to assig a variabel x to obtain the stack address 
    * Is there a higher stack address you could find or does `x` point to the start of the stack? Remember the stack does grow from the end of your address space.
    * Could you show a higher address for this example? If yes how, if not, why?

