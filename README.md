#include<iostream>
using namespace std;
int rats(int r, int unit, int arr[], int n)
{ 
	
	if (n == 0)
	{
		return -1;
	}
	int tot = r * unit, sum=0,count=0;
	for (int i = 0; i < n; i++)
	{
		sum = sum + arr[i];
		count++;
		if (sum >= tot)
		{
			return count;
			break;
		}
	}
	



}


int main() {
	
	int r, unit, n;
	cout << "no.of rats";
	cin >> r;
	cout << "each rat consume";
	cin >> unit;
	cout << "n=";
	cin >> n;
	int arr[10];
	for (int i = 0; i < n; i++)
	{
		cin >> arr[i];
	}
	cout<<rats(r, unit, arr,n);
		
}
