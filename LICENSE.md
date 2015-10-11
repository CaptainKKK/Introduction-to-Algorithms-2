Enter file contents here
// 2.2-2P16.cpp : 定义控制台应用程序的入口点。
#include<iostream>

using namespace std;

int main()
{
	int a[10], i,j,t,temp;
	for(i =0;i<10;i++)
		cin >>a[i];

	for(i =0;i<9;i++)
	{
		j=i;
		t=j+1;
		while(j<10)
		{
			if(t<10&&a[j]< a[t])
				t=j++;
			else
			j++;
		}
		temp=a[i];
		a[i]=a[t];
		a[t]=temp;
	}
		for(i =0;i<10;i++)
		cout <<a[i]<<" ";
	cout <<endl;
	cin >> i;
}

