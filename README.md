#include <iostream>
#include <cstdlib>
using namespace std;
void drill();
int hisob;
int num_right;
int main()
{
	cout << "pratichiskiy mashqlar nechta:";
	cin >> hisob;
	num_right = 0;
	do {
		drill(); hisob--;
	} while (hisob);
		cout << "siz" << num_right << " togri javob berdingiz.\n";
		return 0;
	}
void drill()
{
	int count;
	int a, b,d, c, e, ans;
	a = rand() % 9;
	b = rand() % 9;
	d = rand() % 9;
	c = rand() % 6;
	e = rand() % 12;
	for (count = 0; count < 2; count++){


		cout << "misolning javobi nechi:" << a << "+" << b << "-" << d << "+" << c << "-" << e << " =";
		
		cin >> ans;
		if (ans == a + b - d +c -e) {

			
				cout << "tabriklaymiz sizning javobingiz togri\n";
			num_right++;
			return;
		}
	}
	cout << "siz ozingizni hamma imkoniatlaringizdan foydalandingiz.\n";
	cout << "togri javob" << a + b - d +c-e
		<< '\n';
	
}
