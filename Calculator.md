#include <iostream>

#include <math.h>

#include <cmath>

using namespace std;


void main()

{
    setlocale(0, "");
    
    cout << "[] Бетта калькулятор" << endl << endl;
    
    cout << "[!] Введите опреацию " << endl;
    
    cout << "[+] Сложение" << endl;
    
    cout << "[-] Вычитание" << endl;
    
    cout << "[*] Умножение" << endl;
    
    cout << "[/] Деление" << endl;
    
    cout << "[1] Корень" << endl;
    
    cout << "[2] Деление с остатком" << endl;
    
    cout << "[3] Синус" << endl;
    
    cout << "[4] Косинус" << endl;
    
    cout << "[5] Тангенс" << endl;
    
    char operation;
    float a1, a2, result;
    int aa1, aa2, result1;//тут для целых чисел
    cin >> operation;
    if (operation == '+') {
        cout << "Сложение\nВведите цифры" << endl;
        cout << "Первое число:";
        cin >> a1;
        cout << "Второе число:";
        cin >> a2;
        result = a1 + a2;
        cout << "Результат сложения:" << result << endl;

    }
    else if (operation == '-') {
        cout << "Вычитание\nВведите цифры" << endl;
        cout << "Первое число:";
        cin >> a1;
        cout << "Второе число:";
        cin >> a2;
        result = a1 - a2;
        cout << "Результат вычитания:" << result << endl;
    }
    else if (operation == '*') {
        cout << "Умножение\nВведите цифры" << endl;
        cout << "Первая цифра:";
        cin >> a1;
        cout << "Второе число:";
        cin >> a2;
        result = a1 * a2;
        cout << "Результат умножения:" << result << endl;
    }
    else if (operation == '/') {
        cout << "Деление\nВведите число" << endl;
        cout << "Первое число:";
        cin >> a1;
        cout << "Второе число:";
        cin >> a2;
        result = a1 / a2;
        cout << "Результат Деления:" << result << endl;
    }
    else if (operation == '1') {
        cout << "Корень" << endl;
        cout << "Введите число:";
        cin >> a1;
        result = sqrt(a1);
        cout << "Корень =" << result << endl;
    }
    else if (operation == '2') {
        cout << "Деление с остатком" << endl;
        cout << "Первое число:";
        cin >> aa1;
        cout << "Второе число:";
        cin >> aa2;
        result1 = aa1 % aa2;
        cout << "Result equals" << result1 << endl;
    }
    else if (operation == '3') {
        cout << "Синус числа" << endl;
        cout << "Введите число:";
        cin >> a1;
        result = sin(a1);
        cout << "Синус =:" << result << endl;
    }
    else if (operation == '4') {
        cout << "Косинус числа" << endl;
        cout << "Введите число:";
        cin >> a1;
        result = cos(a1);
        cout << "Косинус =:" << result << endl;
    }
    else if (operation == '5') {
        cout << "Тангенс числа" << endl;
        cout << "Введите число:";
        cin >> a1;
        result = tan(a1);
        cout << "Тангенс =:" << result << endl;
    }
    else {
        cout << "Это бетта калькулятор больше он ничего не умеет" << endl;
    }



}
