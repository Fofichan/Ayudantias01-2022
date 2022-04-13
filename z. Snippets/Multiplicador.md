**Objetivo**

Calcula el producto de dos números SIN UTILIZAR el operador de multiplicación.

**Formato de input**

Dos números enteros, **X** e **Y**.

**Restricciones**

10⁻⁹ <= **X**,**Y** <= 10⁹
Sin utilizar *

**Formato de output**

Imprimir la multiplicación entre **X** e **Y**.

%%
```C++
#include <iostream>
using namespace std;

int main() {

	int X, Y;
	cin >> X >> Y;
	int aux = 0;
	
	while (Y > 0){
		aux = aux + X;
		Y = Y - 1;
	}
	cout << aux << endl;
	return 0;

}
```

%%