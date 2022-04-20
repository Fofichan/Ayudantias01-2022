**Objetivo**

Escribe un programa que calcule e imprima cada paso la suma de la serie: (1 x 1) + (2 x 2) + (3 x 3) + (4 x 4) + ... + (n x n).

**Formato de input**

Un número entero **N**, que indica el n-ésimo término.

**Restricciones**

10⁻⁹ <= **N** <= 10⁹

**Formato de Output**

Guiarse por el siguiente ejemplo. Sea **N** = 5:

1 x 1 = 1
2 x 2 = 4
3 x 3 = 9
4 x 4 = 16
5 x 5 = 25
La suma de la serie es 55

%%
```c++
#include <iostream>
using namespace std;  

int main(){

int n, suma = 0;
cout << " Ingrese el valor para el enésimo término: ";
cin >> n;

for (int i = 1; i <= n; i++){

	suma += i * i;
	cout << i << "*" << i << " = " << i * i << endl;
}

cout << "La suma de la serie es : " << suma << endl;
return 0;
}
```

%%