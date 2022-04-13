**Objetivo**
Dada los coeficientes de una ecuación cuadrática, calcular sus raíces.

**Formato de input**
Un número entero **a** (correspondiente al coeficiente cuadrático), seguido de un espacio y un número entero **b** (correspondiente al coeficiente lineal), seguido de un espacio y un número entero **c** (coeficiente al coeficiente constante).

**Restricciones**
1 <= **a**,**b**,**c** <= 10⁹

**Formato de output**
Raíces asociadas a la ecuación cuadrática, separadas por un salto de línea.

%%
```c++
#include <iostream>
#include <math.h>
using namespace std;

int main(){
	int a,b,c;
	int det;
	float raiz_1, raiz_2;
	cout << "Ingresa los valores de a, b y c: ";
	cin >> a >> b >> c;

	det = b*b - 4*a*c;
	if (det == 0){
		raiz_1 = -b / (2.0*a);
		cout << "Primera raíz: " << raiz_1 << endl;
		cout << "Segunda raíz: " << raiz_1 << endl;
	}
	else if (det > 0){
		raiz_1 = (-b + sqrt(det)) / (2.0*a);
		raiz_2 = (-b - sqrt(det)) / (2.0*a);
		cout << "Primera raíz: " << raiz_1 << endl;
		cout << "Segunda raíz: " << raiz_2 << endl;
	}
	else {
		cout << "Raíces imaginarias." << endl;
	}
}
```
%%
