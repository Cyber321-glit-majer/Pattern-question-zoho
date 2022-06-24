# Pattern-question-zoho

Pattern:

n=5

5____1

_4__2_ 
 
__3__
  
_2__4_
 
1____5 
**

**CODE**

```

#include<bits/stdc++.h>
using namespace std;
 int main()
 {
     int n;
     cin>>n;
     int m=(n+1)/2;
     for(int i=1;i<=n;i++)
     {
         for(int j=1;j<=n;j++)
         {
            if(i==j)
            {
               if(i<m)
               {
                   cout<<n-i+1;
               }
               else
               {
                   cout<<i;
               }
            }
                else if(i+j==n+1)
                {
                   if(i<m)
                   {
                       cout<<i;
                   }
                   else
                   {
                       cout<<j;
                   }
                }
                else
                {
                    cout<<" ";
                }
            
         }
         cout<<endl;
     }
     return 0;
 }
