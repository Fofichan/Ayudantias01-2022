**Objetivo**

Construir un programa que imprima un cuadrilatero (cuadrado o rectángulo) hecho de asteriscos separados por espacios, con largo y ancho a criterio del usuario.

**Formato de input**

Dos números enteros, **N** y **M**, donde **N** es el largo de la figura y **M** es el alto.

**Restricciones**

10⁻⁹ <= **N**,**M** <= 10⁹
 
**Formato de output**

Un cuadrilátero de largo **N** y ancho **M**.

## Ejemplo
```c++
Ingrese largo: 7
Ingrese ancho: 4
*  *  *  *  
*  *  *  *  
*  *  *  *  
*  *  *  *  
*  *  *  *  
*  *  *  *  
*  *  *  *  
```

%%
```c++
#include <iostream>
using namespace std;

int main() {

int N,M;
cout << "Ingrese largo: ";
cin >> N;
cout << "Ingrese ancho: ";
cin >> M;
  

for (int i = 0; i < N; i++) {

	for (int j = 0; j < M; j++) {
		cout << "* ";
	}
	cout << endl;
}

return 0;
}
```
%%
