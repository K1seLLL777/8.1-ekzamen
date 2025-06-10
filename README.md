# 8.1-ekzamen
#include <iostream>
#include <cstring>
using namespace std;

int main() {
    const int MAX_LEN = 100;
    char s[MAX_LEN];
    char c1, c2;

    cout << "Введіть рядок: ";
    cin.getline(s, MAX_LEN);

    cout << "Введіть символ, який потрібно знайти: ";
    cin >> c1;

    cout << "Введіть символ для заміни: ";
    cin >> c2;

    for (int i = 0; i < strlen(s); i++) {
        if (s[i] == c1) {
            s[i] = c2;
        }
    }

    cout << "Змінений рядок: " << s << endl;

    return 0;
}
