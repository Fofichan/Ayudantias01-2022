**Objetivo**

Escriba un programa que imprima un triangúlo rectángulo usando asteríscos.

**Formato de input**

Un número **N**, que indica el número de filas.

**Restricciones**

10⁻⁹ <= **N** <= 10⁹

**Formato de output**

Un triángulo rectángulo de altura **N** y base **N**, hecha con asteríscos

## Ejemplo
Ingrese un número: 5
```c++
*
**
***
****
*****
```

%%
```c++
#include <iostream>
using namespace std;

int main() {
	int N;
	cout << "Ingrese un número: ";
	cin >> N;

	for(int i=1; i<=N; i++) {
	
		for(int j=1; j<=i; j++){
			cout<<"*";
		}
	cout<<endl;
	}
	return 0;
}
```
%%