#include <iostream>
#include <cmath>
using namespace std; 

int main()
{
  double x1, x2, x3, y1, y2, y3; 
  cin>>x1>>y1>>x2>>y2>>x3>>y3; 
  double a = sqrt((x1-x2) * (x1-x2) + (y1-y2)*(y1-y2));
  double b = sqrt((x3-x2) * (x3-x2) + (y3-y2)*(y3-y2)); 
  double c = sqrt((x1-x3) * (x1-x3) + (y1-y3)*(y1-y3)); 
  double p = 0.5*(a+b+c);
  cout<<sqrt(p*(p-a)*(p-b)*(p-c)); 
  return 0;
}

