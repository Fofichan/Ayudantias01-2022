**Objetivo**

Calcular la diferencia (resta) entre la suma máxima y suma mínima de **N** - **M** elementos de un arreglo dado.

**Formato de input**

En la primera línea, un entero positivo **N**, que corresponde al tamaño del arreglo y un entero positivo **M**.
En la segunda línea, **N** enteros, que corresponden a los elementos del arreglo.

**Restricciones**

0 < **N**,**M**<= 10⁹

**Formato de output**

El resultado de la resta entre la suma máxima y la mínima.

### Input:
```c++
5 1
1 2 3 4 5
```
### Output:
```c++
4
```

## Ayuda
Sea **M** igual a  1 y **N** igual 5, se debe calcular la máxima y mínima suma usando **5**-**1** = 4 elementos del arreglo. La máxima suma corresponde a los mayores 4 elementos , y la mínima súma corresponde a los menores 4 elementos.

%%
### Solución
```c++
#include <iostream>
using namespace std;

int main(){

	int n;
	cin >> n;
	int m;
	cin >> m;
	int arr[n];
	for(int i=0; i<n; i++){
		cin>>arr[i];
	}

	int diff=n-m;

	for(int i=0; i<n-1; i++){

	bool aux=false;
	for(int j = 0; j < n-1; j++){
		if(arr[j] > arr[j+1]){
			swap(arr[j], arr[j+1]);
			aux=true;
		}
	}
		if(aux==false){
			break;
		}
	}
	  
	int maxsum=0;
	int minsum=0;
	for(int i = 0; i < diff; i++){
		minsum = minsum + arr[i];
	}
	
	for(int i = n-1; i >= n-diff; i--){
		maxsum = maxsum + arr[i];
	}
	
	int d = maxsum-minsum;
	cout << d << endl;

return 0;
}
```
%%