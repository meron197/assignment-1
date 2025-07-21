assignment-1
#include <iostream>
#include <string>
using namespace std;

class rectangle {
private:
    int width, length;

public:

    rectangle(int l, int w) {
        length = l;
        width = w;
    }

    void display() {
        cout << "Length: " << length << endl;
    }


    int area() {
        return length * width;
    }
};

int main() {
    int length, width;  

     cout << "Enter the length of the rectangle: ";
    cin >> length;
    cout << "Enter the width of the rectangle: ";
    cin >> width;

    rectangle r(length, width);
  

    cout << "Area: " << r.area() << endl;

    return 0;
}
