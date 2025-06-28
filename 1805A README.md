#include<bits/stdc++.h>
using namespace std;

typedef long long int ll;
typedef unsigned long long int llu;
typedef double dl;

#define endl '\n'
#define PI acos(-1)
#define vi vector<int>
#define vll vector<ll>
#define vii vector<pair<int,int>>


int main()
{
  ios_base::sync_with_stdio(0);cin.tie(0);cout.tie();
  ll t,n,i;
  cin>>t;
  while(t--)
  {
      cin>>n;
      ll arr[n];
      for(i=0; i<n; i++)
      {
          cin>>arr[i];
      }
      ll s = arr[0];
      for(i=1; i<n; i++)
      {
          s = arr[i]^s;
      }
      if(n%2==1)
      {
          cout<<s<<endl;
      }else{
        if(s==0){
            cout<<0<<endl;
        }else{
           cout<<-1<<endl;
          }
      }

  }

    return 0;
}

