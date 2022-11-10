# Code-I-wrote-as-an-undergraduate2
For 100,000 lines of code
//双数组写数组的循环后移问题//
```
#include <iostream>
using namespace std;
int main()
{
	int n, m;
	int a[10];
	int b[10];
	cin >> n >> m;
	for (int i = 0; i < n; ++i)
	{
		cin >> a[i];
		b[i] = a[i];
	}

	
	for (int i = 0; i < n; ++i)
	{
		int x = i + m;
		if (x> n - 1)
		{
			for (int t = 1;; t++)
			{
				x -= n;
				if (x < n)
				{
					break;
				}
			}
		}
		a[x] = b[i];
	}

	for (int i = 0; i < n; ++i)
	{
		cout << a[i] << ' ';
	}
	return 0;
}
```
