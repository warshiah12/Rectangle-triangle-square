# Rectangle-triangle-square
#displaying area of rectangle, triangle, square
#include<iostream>
using namespace std;
int main()
{
	double sq, rect, tri, l, w;   //declaring variables with datatype double
	cout << "Enter the length and width : " << endl;
	cin >> l >> w;
	while (cin.fail() != 0)  //if user enters any other character instead of number then it will ask the user to enter the length and width again 
	{
		cout << "\aInvalid Command.\nEnter length and width : ";
		cin.clear();
		cin.ignore();
		cin >> l >> w;
	}
	rect = l * w;   //formula to calculate area of rectangle
	tri = 0.5 * l * w;   //formula to calculate area of triangle
	sq = l * l;   //formula to calculate area of square
	cout << "Area of Rectangle = " << rect << endl;  
	cout << "Area of Triangle =  " << tri << endl;
	cout << "Area of Square =    " << sq << endl;
	return 0;
}
