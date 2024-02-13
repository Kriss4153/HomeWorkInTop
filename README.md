//Палиндром
#include<iostream>
using namespace std;

void main()
{
	setlocale(LC_ALL, "Russian");
	int number;
	cout << "Введите число: "; cin >> number;
	int buffer = number;
	int reverse = 0;
	while (buffer > 0)
	{
		reverse *= 10;
		reverse += buffer % 10;
		buffer /= 10;
	}
	
	if (reverse == number)
	{
		cout << "Палиндром" << endl;
	} 
	else
	{
		cout << "Обычное число" << endl;
	}
}# HomeWorkInTop
