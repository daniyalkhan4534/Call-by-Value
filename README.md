Call By Value:

The call by value method of passing arguments to a function copies the actual value of an argument into the function. C programming uses call by value to pass arguments.
It means the code within a function cannot alter the arguments used to call the function.

![image](https://user-images.githubusercontent.com/127819492/234473313-853d0307-6936-46a6-bd35-9919fec38c39.png)


Actual parameters: The parameters that appear in function calls. Formal parameters: The parameters that appear in function declarations.

In call by value method, the value of the actual parameters is copied into the formal parameters. The value of the variable is used in the function call in the call by value method.
We can not modify the value of the actual parameter by the formal parameter.
Different memory is allocated for actual and formal parameters since the value of the actual parameter is copied into the formal parameter.
Code:

#include <windows.h> #include<stdio.h>

void disp(int);

int main()
{
	int x=2;
	disp(x);
	printf("%d",x);
}
void disp(int a)
{
	printf("%d",a);
	a=a+1;
}
