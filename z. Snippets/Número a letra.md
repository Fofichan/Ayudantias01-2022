**Objetivo**
Dado un número positivo **n**, realice lo siguiente:
- SI 1 <= **n** <= 9, imprima en minúscula la palabra correspondiente a ese numero (ej, "uno" para 1, "dos" para 2, etc.)
- SI **n** > 9, imprimir "Mayor a 9".

**Formato de input**
Un número entero, **n**.

**Restricciones**

1 <= **n** <= 10⁹

**Formato de output**
Si **n** está entre 1 y 9, imprimir el correspondiente en minúscula. En caso contrario, imprimir mayor a 9.

%%
```c++
#include <iostream>
using namespace std;  

int main(){

	int n;
	cin >> n;

	if (n > 9){
		cout << "Mayor a 9";
	}
	else if (n > 8) {
		cout << "Nueve";
	}
	else if (n > 7) {
		cout << "Ocho";
	}
	else if (n > 6) {
		cout << "Siete";
	}
	else if (n > 5) {
		cout << "Seis";
	}
	else if (n > 4){
		cout << "Cinco";
	}
	else if (n > 3){
		cout << "Cuatro";
	}
	else if (n > 2){
		cout << "Tres";
	}
	else if (n > 1){
		cout << "Dos";
	}
	else if (n > 0){
		cout << "Uno";
	}
	else {
		cout << "Input inválido.";
	}
	
return 0;
}

```
%%