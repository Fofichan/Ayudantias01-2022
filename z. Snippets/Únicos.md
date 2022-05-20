**Objetivo**

Escribe un programa que busque e imprima todos los números únicos dado un arreglo de elementos.

**Formato de input**

No hay input.

**Formato de output**

```c++
Números del arreglo: 1 5 7 5 8 9 11 11 2 5 6
Elementos únicos del arreglo: 1 5 7 8 9 11 2 6
```

## Ayuda
```c++
#include <iostream>
using namespace std;
  
int main(){
	int arreglo[] = {1, 5, 7, 5, 8, 9, 11, 11, 2, 5, 6};
	int size = sizeof(arreglo)/sizeof(arreglo[0]);
	cout << "Números del arreglo: ";
	for (int i=0; i < size; i++){
		cout << arreglo[i] <<" ";
	}
	cout <<"\nElementos únicos del arreglo: ";

	//tu código aquí.

return 0;

}
```

%%
```c++
	for (int i=0; i<size; i++){
		int j;
		for (j=0; j<i; j++){
			if (arreglo[i] == arreglo[j]){
			break;
			}
			if (i == j){
				cout << arreglo[i] << " ";
			}
		}
	}
	cout << endl;
```
%%
