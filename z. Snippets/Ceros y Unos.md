**Objetivo**

Construye un programa que, mediante una función, ubique los ceros y unos de un arreglo, a la izquierda y a la derecha, respectivamente.

**Formato de output**

```c++
Arreglo original: 0 1 0 0 1 1 1 0 1 0 
Arreglo ordenado: 0 0 0 0 0 1 1 1 1 1 
```


## Ayuda: 
```c++

int arr[] = {0, 1, 0, 0, 1, 1, 1, 0, 1, 0};
int n = sizeof(arr)/sizeof(arr[0]);

```

%%
```c++
#include <iostream>
using namespace std;  

void cerouno(int arr[], int n){
	int aux = 0;

	for (int i = 0; i < n; i++) {
		if (arr[i] == 0){
			aux++;
		}
	}

	for (int i = 0; i < aux; i++){
		arr[i] = 0;
	}
	
	for (int i = aux; i < n; i++){
		arr[i] = 1;
	}
}

int main(){

	int arr[] = {0, 1, 0, 0 , 1, 1, 1, 0, 1, 0};
	int n = sizeof(arr)/sizeof(arr[0]);
	cout << "Arreglo original: ";
	  
	for (int i=0; i < n; i++){
		cout << arr[i] <<" ";
	}

	cerouno(arr, n);

	cout << endl;
	cout << "Arreglo ordenado: ";
	for (int i=0; i < n; i++){
		cout << arr[i] <<" ";
	}
	cout << endl;

return 0;

}
```
%%