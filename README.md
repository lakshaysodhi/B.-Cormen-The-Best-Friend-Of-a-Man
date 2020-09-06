# B.-Cormen-The-Best-Friend-Of-a-Man
#include <bits/stdc++.h>
using namespace std;
 
int main() {
 
    int n,k;
    cin>>n>>k;
    vector<int> A(n);
    for(int i=0;i<n;i++){
        cin>>A[i];
    }
    int additional=0,x;
 
    for(int i=1;i<n;i++){
        x=(k-A[i]-A[i-1]);
        if(x>0){
        A[i]+=x;
        additional+=x;
        }
    }
    cout<<additional<<endl;
    for(int i=0;i<n;i++){
        cout<<A[i]<<" ";
    }
 
}
 
