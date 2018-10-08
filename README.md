/*Christie Carranza*/

#include<stdio.h>
#include<math.h>
int main()
{
int n, count=0, loop1=0;

printf("Enter n: \n");
scanf("%d", &n);


for(count=1; count <=n; count++)
    {
     loop1+=count*(count+1);
    }
  count=1;
  double loop2=0;
while(count<=n)
    {
    loop2+=1.0/(count*(count+1));
    count++;
    }
  double loop3=0;
  count=1;

do
    {
      loop3+=1/(pow(2,count));
      count++;
    }
while (count<=n);
   int F1=n*(n+1)*(n+2)/3;
   double F2=1-1.0/(n+1);
   double F3=1-1.0/(pow(2,n));


printf("For Loop\n\tLoop Result= %d\n\tFormula= %d\n", loop1, F1);
printf("While Loop\n\tLoop Result= %f\n\tFormula= %f\n", loop2, F2);
printf("Do while Loop\n\tLoop Result= %f\n\tFormula= %f\n", loop3, F3);
return 0;
}

