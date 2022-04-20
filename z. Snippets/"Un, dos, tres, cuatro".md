**Objetivo**

Escriba un programa que calcule e imprima todas las combinaciones de tres dígitos únicos, usando 1, 2, 3 y 4. Además indique el total de combinaciones.

**Formato de input**

No hay input.

**Restricciones**

Sólo combinaciones únicas de tres dígidos.
Sólo usar 1, 2, 3 y 4.
No pueden haber dígitos repetidos en cada combinación.

**Formato de output**
```c++
123 124 132 134 142 143 213 214 231 234 241 243 312 314 321 324 341 342 412 413 421 423 431 432
El total de combinaciones es 24
```
%%
```c++
#include <iostream>
using namespace std;

int main(){
	int total = 0;
	for(int i = 1; i <= 4; i++){
		for(int j = 1; j <= 4; j++){
			for(int k = 1; k <= 4; k++){
				if(k != i && k != j && i != j){
					total++;
					cout<<i <<j<<k<<" ";
				}
			}
		}
	}
	cout << endl << "El total de combinaciones es: " << total << endl;
	return 0;
}

```
%%