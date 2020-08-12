/*# hrishi*/
#include<stdio.h>
#include<sys/types.h>
void forkexample()
{
  //child process because return zero value
  if(fork()==0)
  {
    printf("hello child\n");
  }
  //parent process because return non zero value
  else
  {
    printf("hello form parent\n");
  }
}
int main()
{
  forkexample();
  return 0;
}
