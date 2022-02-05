# CSES-Intro-3
Repetitions Solution

#include<bits/stdc++.h>
using namespace std;
 
int main(){
    
ios_base::sync_with_stdio(false);
cin.tie(NULL);
 
    string s;
    cin>>s;
 
    int mx=INT_MIN;
    int ct=1;
 
    int sz=s.size();
    for (int i = 0; i < sz-1; i++)
    {
        if(s[i]==s[i+1]){
            ct++;
        }
        else{  
            mx=max(mx,ct);
            ct=1;
        }
    }
    mx=max(mx,ct);
    cout<<mx<<endl;
return 0;
}  
