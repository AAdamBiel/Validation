#include <iostream>

using namespace std;

void fibonacci(int n) {
    int t1 = 0, t2 = 1, nextTerm;
    
    cout << "Fibonacci Series: " << t1 << ", " << t2;
    for (int i = 2; i < n; i++) {
        nextTerm = t1 + t2;
        cout << ", " << nextTerm;
        t1 = t2;
        t2 = nextTerm;
    }
}

int main() {
    int num;
    cout << "Enter the number of terms: ";
    cin >> num;
    fibonacci(num);
    return 0;
}
