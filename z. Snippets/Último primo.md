**Objetivo**

Escribe un programa que encuentre el último número primo presente antes de un número dado.

**Formato de input**

Un número entero **N**.

**Restricciones**

10⁻⁹ <= **N** <= 10⁹

**Formato de output**

El último número primo identificado antes de **N**

## Ejemplo
Ingrese un número: 46

El último primo es: 43

#### Explicación:

1, **2**, **3**, 4, **5**, 6, **7**, ... , **41**, 42, **43**, 44, 45, 46

%%
```c++
#include <iostream>
using namespace std;
int main(){
	int N, ctr = 0;
	cout << "Ingrese un número: ";
	cin >> N;
	
	for (int n = N - 1; n >= 1; n--){  
		for (int m = 2; m < n; m++){
			if (n % m == 0)
			ctr++;
		}
		if (ctr == 0){
			if (n == 1){
				cout << "No hay números primos menores a 2." <<endl;
			break;
			}
		cout << n << " es el último número primo antes de " << N << endl;
		break;
		}
	ctr = 0;
	}
	return 0;
}
```
%%