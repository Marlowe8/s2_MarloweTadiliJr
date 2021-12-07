# s2_MarloweTadiliJr

	#include <iostream>
	#include <string>
	#include <iomanip>
	using namespace std;


	int main() {
		string User;
		int i, Input;
		int factorial = 1;
		int Inputf;
		cout << "Enter your full name: ";
		getline(cin, User);
		cout << "Enter any number: "; cin >> Input;
		if (cin.fail()) {
			cout << "Error" << endl;
			return 0;
		}
		Inputf = Input;
		do {
			factorial *= Inputf;
			Inputf--;
		} while (Inputf > 1);//Factorial
		cout << "Factorial: " << factorial << endl;
		cout << "Table" << endl;
		for (i = 0; i <= 10; i++)//Table input * 1-10;
		{
			cout << Input << " * " << i << " = " << Input * i << endl;

		}
		int j = 0;
		cout << "Exponent power" << endl;
		while (j <= 10)//Exponent
		{
			cout << Input << "^" << j << " = " << pow(Input,j) << endl;
			j++;

		}
		return 0;
	}
