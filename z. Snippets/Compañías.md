Una compañia distribuidora de aciete para vehículos motorizados, ha decidido mecanizar el control de ventas en uno de sus puntos de distribución. La compañia comercializa tres tipos de aceites; aceite tipo 1 (de primera), cuyo valor por litro es de $5.000 aceite, tipo 2 (de segunda) con precio de $4.000 por litro y aceite tipo 3 (de tercera) con costo de $3.000 por litro.
Se solicita implementar una solución computacional, en lenguaje C++, que permita registrar las ventas que realiza esta compañía por cada tipo de aceite.
**Se pide:**
A. Hacer un programa que lea desde teclado por cada tipo de aceite el total de litros vendidos durante cada día del mes. El programa debe generar los arreglos **T1**, **T2** y **T3**, de largo 31 con valores correspondientes a cada tipo de aceite cada día.
B. Programar la función **TotalFacturado(T1, T2, T3, N)**, que calcule e imprima el total facturado por cada tipo de aceite y retorne el total general vendido.
C. Programar la función **MayorDemanda( T1, T2, T3, N)** que retorne el tipo de combustible con mayor cantidad de litros vendidos.
D. Agregar al programa el llamado a las funciones descritas en los puntos anteriores, imprimiento el **total vendido en pesos** y **el tipo de aceite con mayor demanda**.


%%
```c++
#include <iostream>
#include <string>
#include <iomanip>
using namespace std;

float totalFacturado(float T1[], float T2[], float T3[], int N){

	float res;
	float tfact_dia[3]={0,0,0};
	for (int i = 0; i < N; i++){
		tfact_dia[0] +=T1[i];
		tfact_dia[1] +=T2[i];
		tfact_dia[2] +=T3[i];
	}
	
	cout << "Litros Tipo 1: " << tfact_dia[0] << " Facturado: " << tfact_dia[0]*5000 <<endl;
	cout << "Litros Tipo 2: " << tfact_dia[1] << " Facturado: " << tfact_dia[1]*4000 <<endl;
	cout << "Litros Tipo 3: " << tfact_dia[2] << " Facturado: " << tfact_dia[2]*3000 <<endl;

	res = tfact_dia[0]*5000 + tfact_dia[1]*4000 * tfact_dia[2]*3000;
	return res;
}

int mayorDemanda (float T1[], float T2[], float T3[], int N){
	
	float tfact_dia[3]={0,0,0};
	for (int i = 0; i < N; i++){
		tfact_dia[0] +=T1[i];
		tfact_dia[1] +=T2[i];
		tfact_dia[2] +=T3[i];
	}

	if(tfact_dia[0] > tfact_dia[1] && tfact_dia[0] > tfact_dia[2]){
		return 1;
	}
	else if(tfact_dia[1] > tfact_dia[0] && tfact_dia[1] > tfact_dia[2]){
		return 2;
	}
	else
		return 3;
}

int main(){
	int N = 5;
	float T1[N], T2[N],T3[N];
	cout << "Ingrese los datos:" <<endl;
	for (int i = 0; i < N; i++){
		cout <<"Ingrese litros de día " << i+1 << ":" << " "<<endl;
		cout <<"Tipo 1: ";
		cin>>T1[i];
		cout <<"Tipo 2: ";
		cin>> T2[i];
		cout <<"Tipo 3: ";
		cin>> T3[i];
	}

	float TFacturado = totalFacturado(T1,T2,T3,N);
	float idMayor = mayorDemanda(T1,T2,T3,N);

	cout << "Total Facturado: " << TFacturado <<endl;
	cout << "Aceite con mayor demanda: " << idMayor <<endl;
	
	return 0;
}

```
%%




