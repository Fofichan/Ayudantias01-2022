*Año bisiesto es aquel año divisible entre 4, salvo que sea año secular - último de cada siglo, terminando en «00»-, en cuyo caso también ha de ser divisible entre 400.*

**Objetivo**

Escribir un problema que identifique si un año **n** dado es año bisiesto o no.

**Formato de input**

Un número entero **n**.

**Restricciones**

1 <= **n** <= 10⁹

**Formato de output**

Indicar si el número ingresado corresponde a un año bisiesto o no.

%%
```c++
#include <iostream>
using namespace std;

int main(){
	int n;
	cout << "Ingrese un año: ";
	cin >> n;
	if ((n % 400) == 0){
		cout << n << " es un año bisiesto." << endl;
	}
	else if ((n % 100) == 0){
		cout << n << " no es un año bisiesto." << endl;
	}
	else if ((n % 4) == 0){	
		cout << n << " es un año bisiesto." << endl;
	}
	else {
		cout << n << " no es un año bisiesto." << endl;
	}
return 0;
}
```
%%