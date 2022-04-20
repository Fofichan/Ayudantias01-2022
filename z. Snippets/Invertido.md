**Objetivo**

Escribe un programa que imprima al revés un número ingresado.

**Formato de input**

Un número entero **N**.

**Restricciones**

10⁻⁹ <= N <= 10⁹

**Formato de output**

El número **N** pero invertido

## Ejemplo

Ingrese un número: 12345
El número invertido es: 54321

%%
```c++
#include <iostream>
using namespace std; 

int main(){

int N, aux, sum = 0;
cout << "Ingrese un número: ";
cin >> N;
for (int t = N; N != 0; N = N / 10){
	aux = N % 10;
	sum = sum * 10 + aux;
}
cout << "El número invertido es: " << sum << endl;
return 0;
}
```