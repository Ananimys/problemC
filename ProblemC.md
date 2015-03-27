#include<iostream>
using namespace std;
int main()
{
int a,b,k,schet;
cin»a»b»k;
int x=a-1;
int y=b+1;
int mass[51000];
int m=0;
for(int i=x; i<=y; i++)
{
if(i%k==0) 
{
mass[m]=i; i+=k-1; m++;
}
}
schet=m*2;
if(mass[0]==x ||mass[0]==a) schet--;
if(mass[m-1]==y||mass[m-1]==b) schet--;
cout « schet;
return 0;
}
