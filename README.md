# Chef-and-Happy-String

#include <iostream>
#include<string.h>
using namespace std;

int main() {
	int n;
	cin>>n;
	while(n--)
	{
	    string a;
	    int count=0;
	    cin>>a;
	    for(int i=0;i<a.size();i++)
	    {
	        if(a[i]=='a'||a[i]=='e'||a[i]=='i'||a[i]=='o'||a[i]=='u')
	        {
	            count++;
	            if(count>2)
	            {
	            cout<<"Happy"<<endl;
	            break;
	            }
	            
	        }
	        else
	        count=0;
	    }
	    if(count<=2)
	    cout<<"Sad"<<endl;
	}
	return 0;
}
