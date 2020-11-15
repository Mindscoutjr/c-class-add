#include <iostream>
using namespace std;

class item {
    int a, b;
  public:
    void set_values (int,int);
    int area() {return a+b;}
};

void item::set_values (int x, int y) {
  a = x;
  b = y;
}

int main () {
  item sum;
  sum.set_values (3,4);
  cout << "Sum: " << sum.area();
  return 0;
}
