#include <iostream>
#include <iomanip>
#include <time.h>

using namespace std;

void Input(int* a, const int n, int i)
{
	cout << "a[" << i << "] = ";
	cin >> a[i];
	if (i < n - 1)
		Input(a, n, i + 1);
	else
		cout << endl;
}

template<typename T>
void Input(T* a, const int n, int i)
{
	cout << "a[" << i << "] = ";
	cin >> a[i];
	if (i < n - 1)
		Input(a, n, i + 1);
	else
		cout << endl;
}

void Print(int* a, const int n, int i)
{
	cout << setw(4) << a[i];
	if (i < n - 1)
		Print(a, n, i + 1);
	else
		cout << endl;
}

template<typename T>
void Print(T* a, const int n, int i)
{
	cout << setw(4) << a[i];
	if (i < n - 1)
		Print(a, n, i + 1);
	else
		cout << endl;
}

int Sum(int* a, const int n, int i, int S)
{
	S += a[i] * a[i];
	if (i < n - 1)
		return Sum(a, n, i + 1, S);
	else
		return S;
}

template<typename T>
T Sum(T* a, const int n, int i, T S)
{
	S += a[i] * a[i];
	if (i < n - 1)
		return Sum(a, n, i + 1, S);
	else
		return S;
}

int main()
{
	int n;
	cout << " " << "n = ";
	cin >> n;
	int* a = new int[n];

	Input<int>(a, n, 0);
	Print<int>(a, n, 0);

	cout << "S = " << Sum<int>(a, n, 0, 0) << endl;

	return 0;
}
