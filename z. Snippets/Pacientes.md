**Objetivo**

Construir un programa que pregunte por el peso de 10 pacientes en un clínica. Para cada paciente, decir lo siguiente:
- Si pesa menos de 60 Kg, "Necesita dieta de nutrición."
- Si pesa de 60 hasta 70 Kg, "Está en su peso ideal."
- SI pesa más de 70 Kg, "Necesita reducir su dieta en calorías."
Indicar al final cuántos pacientes por cada categoría existen.

**Formato de input**

Un número **N** que indique el peso de un paciente, hasta 10 pacientes.

**Restricciones**

10⁻³⁸ <= **N** <= 10³⁸

**Formato de output**

Por cada peso de paciente ingresado, indicar alguna de las categorías a la que el paciente pertenecezca. Al llegar a 10 pesos de pacientes, indicar el total de pacientes por categoría.

%%
```c++
#include <iostream>
using namespace std;

int main(){
	float peso = 0.0;
	int a = 0;
	int b = 0;
	int c = 0;
	int t = 0;

	while(t <10){
		cout << "Ingresa el peso del paciente: ";
		cin >> peso;
		t++;
		if(peso < 60){
			cout << "Necesita dieta de nutrición." <<endl;
			a++;
		}
		else if(peso >= 60 && peso < 70){
			cout << "Está en su peso ideal." << endl; 
			b++;
		}
		else {
		cout << "Necesita reducir su dieta en calorías." << endl;
		c++;
		}	
	}
	cout << "\nDieta de nutrición: " << a << endl;
	cout << "Peso ideal: " << b << endl;
	cout << "Reducir calorías: " << c << endl;

	return 0;
}
```
%%