**Objetivo**
Identificar si es que, según tres ángulos, conforman un triángulo válido.

**Formato del input**
Tres números enteros, **a**, **b** y **c**, separados por un espacio.

**Formato del output**
Si los ángulos son válidos, imprimir por consola "El triángulo es válido". En caso contrario, imprimir por consola "El triángulo no es válido.".


%%
```c++
#include<iostream>
using namespace std;
int main(){
	int a;
	int b;
	int c;
	cout << "Ingresa tres ángulos de un triángulo: " << endl;
	cin >> a >> b >> c;
	int sum=a+b+c;
	if(sum==180 && a!=0 && b!=0 && c!=0){
		cout << "El triángulo es válido." << endl;
	}
	else{
		cout << "El triángulo no es válido." << endl;
	}
	return 0;
}
```
%%