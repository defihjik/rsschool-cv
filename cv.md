# My CV

I am ***Eugeniy Kakhno***. 

My telephone number is ***+375 33 392 30 91***. My email is ***k.2014.evgeniy@gmail.com***.

***My goal is to become a Front-end developer.***  
My strengths: ***determination** and **ability to work in a team***.

I know the old programming language ***Pascal***, but I haven’t used it for a long time. Instead, I use ***C++*** and solve algorithmic problems in it.

This is an example of ***my*** code: 
```
#include <bits/stdc++.h>
using namespace std;

int main()
{
  freopen("GLUE.IN","r",stdin);
  freopen("GLUE.OUT","w",stdout);
  int x[4]={0,0,1,-1};
  int y[4]={1,-1,0,0};
  int q[3][10204],k,tek,tx,ty,t,i,w,j,n,m,z;
  int a[101][101];
  cin>>n>>m;
  int l;
  cin>>l;
  for (i=1; i<=n; i++)
    for (j=0; j<m; j++)
    cin>>a[i][j];
    w=0;
  for (i=1; i<=n; i++)
    for (j=0; j<m; j++)
    if (a[i][j]!=-1)
  {
    w=a[i][j];
    a[i][j]=-1;
    q[1][1]=i;
    q[2][1]=j;
    z=1;
    k=2; tek=0;
    while (k>tek)
    {
        tek++;
        tx=q[1][tek];
        ty=q[2][tek];
        for (t=0; t<4; t++)
          if ((tx+x[t]>=1)&&(tx+x[t]<=n)&&(ty+y[t]>=0)&&(ty+y[t]<m))
          if (a[tx+x[t]][ty+y[t]]==w)
        {
            q[1][k]=tx+x[t];
            q[2][k]=ty+y[t];
            z++;
            a[tx+x[t]][ty+y[t]]=-1;
            k++;
        }
    }
    if (z!=l) {cout<<"Wrong answer"; return 0;}
  }
  cout<<"OK";
}

``` 

