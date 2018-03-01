#include <bits/stdc++.h>

using namespace std;

int main()
{
    ios_base::sync_with_stdio(0); cin.tie(0); cout.tie(0);
    int n,l;
    int arr[50];
    cin>>n;
    for(int i=0; i<n; i++)
    {
        int cnt=0;
        cin>>l;
        for(int j=0; j<l; j++)
        {
            cin>>arr[j];
        }

        for(int k=0; k<l; k++)
        {
            int x;
            x=arr[k];
             for(int m=k; m<l; m++)
             {
                if(x>arr[m])
                    cnt++;
             }
        }

        cout<<"Optimal train swapping takes "<<cnt<<" swaps."<<endl;

    }
    return 0;
}
