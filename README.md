# 6-lang-one
/* Program to demonstrate time taken by loop */
#include<time.h>
#include<stdio.h>
void main()
{ int c=0;/*count var*/
clock_t t;
t=clock();/*starts the clock*/
for(int i=0;i!=-1;i++)
{
c++;
t=clock()-t;/* time gets updated each iteration*/
double time_taken=((double)t)/CLOCKS_PER_SEC;/*time taken calculated by division by ticks per sec*/
if(time_taken==1)
break;
}
printf("%d",c);
}/*end of program*/
