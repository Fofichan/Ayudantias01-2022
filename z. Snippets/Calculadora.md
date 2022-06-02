**Objetivo**

Crea una calculadora que reciba dos números y un operador matemático, y que imprima el resultado de la operación matemática.

**Formato de input**

Un número real **a**, seguido de un operador matemático y un número real **b**.

**Restricciones**

10⁻³⁸ <= **a**,**b** <= 10³⁸
Las operaciones matemáticas **deben** estar expresadas dentro de funciones.
Operaciones matemáticas: '+', '-', '/' ,'^' y '*'.
**Formato de output**
El número resultante de la operación matemática.


## Ejemplo de output
```c++
4 / 7
0.571428571
```


%%
```c++
#include <iostream>
#include <math.h>
using namespace std;

float calc(float a, char op, float b){

	if(op == '+'){
		return a + b;
	}
	else if(op == '-'){
		return a - b;
	}
	else if(op == '*'){
		return a * b;
	}
	else if(op == '/'){
		if(b !=0){
			return a/b;
		}
		else{
			cout << "div por cero";
			return 0;
		}
	}
	else if(op == '^'){
		return pow(a,b);
	}
	else{
		cout << "Op. inválida";
		return 0;
	}
}

int main(){

float x,z;
char y;
cin >> x;
cin >> y;
cin >> z;
cout << calc(x,y,z) << endl;
return 0;
}
```

%%
