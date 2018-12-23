# UTC-BTC
UTC-BTC
#include<stdio.h>
int main()
{
  int x;
  int h,m ;
  scanf("%d",&x);

  if (x-800<0)
    x=2400+x-800;
  else 
    x-=800;
  if (x>=0&&x<=2359)
  {
    if (x>0&&x<100)
      {m=x;h=-1;}
      else if (x>=100)
        {h=x/100;m=x%100; }
  }
      else return 0;
    if (h>0&&m<10)
      printf("%d0%d",h,m);
      else if (h>0&&m>=10)
        printf("%d%d",h,m);
          else if (h<0)
            printf("%d",m);
}
