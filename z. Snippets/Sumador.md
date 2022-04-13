**Objetivo**

Construye un programa que sume sólo números positivos y ceros. Si el usuario ingresa un número negativo, imprime la suma y termina el programa.

**Formato de input**

Un número entero **N**. Si el número es positivo o cero, súmalo y solicita al usuario que ingrese otro número.

**Restricciones**

10⁻⁹ <= N <= 10⁹

**Formato de output**

La suma de todos los números **N** que ha ingresado el usuario.

%%
```c++
#include <iostream>
using namespace std;

int main() {
    int N;
    int suma = 0;

    cout << "Ingresa un número: ";
    cin >> N;

    while (N >= 0) {
        suma += N;
        cout << "Ingresa un número: ";
        cin >> N;
    }
    
    cout << "\nLa suma es: " << suma << endl;

    return 0;
}
```
%%