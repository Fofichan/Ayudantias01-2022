**Objetivo**

Escribe un programa que encuentre los números repetidos en un arreglo.

**Formato de input**

Sin input.

**Formato de output**


```c++
Números del arreglo: 1 2 3 5 5 7 8 8 9 9 2
Números repetidos: 2 5 8 9
```

## Ayuda
```c++
#include <iostream>
using namespace std;
int main(){
	int numeros[] = {1, 2, 3, 5, 5, 7, 8, 8, 9, 9, 2};
	int size = sizeof(numeros)/sizeof(numeros[0]);
	cout << "Números del arreglo: ";
	for (int i = 0; i < size; i++){
		cout << numeros[i] <<" ";
	}
	cout << "\nElementos repetidos: ";

	for(int i = 0; i < size; i++){
		for(int j = i+1; j < size; j++){
			if(numeros[i] == numeros[j]){
				cout << numeros[i] << " ";
			}
		}
	}


return 0;

}
```

%%
```c++
	for(int i = 0; i < size; i++){
		for(int j = i+1; j < size; j++){
			if(numeros[i] == numeros[j]){
				cout << numeros[i] << " ";
			}
		}
	}

cout <<endl;
```
%%