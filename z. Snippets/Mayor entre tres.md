**Objetivo**
Identifica cual de los tres numeros ingresados es el mayor.

**Formato de input**

Tres números enteros; **a**, **b** y **c**, separados por un espacio.

**Restricciones**

-10⁹ <= **a**, **b**, **c** <= 10⁹

**Formato de output**

Imprimir por consola "El número mayor entre los tres es", seguido de un espacio y el número mayor entre los tres.

%%
```c++
#include <iostream>
using namespace std;
int main(){
	int x;
	int y;
	int z;
	cout <<"Ingresa tres números: ";
	cin >> x >> y >> z;
	if(x>=y && x>=z){
		cout << "El número mayor entre los tres es: " << x;
	}
	if(y>=x && y>=z){
		cout << "El número mayor entre los tres es: " << y;
	}
	if(z>=x && z>=y){
		cout << "El número mayor entre los tres es: " << z;
	}
	return 0;
}
```
%%