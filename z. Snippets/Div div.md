**Objetivo**

Escriba un programa C++ que:
- Calcule encuentre los números enteros divisibles por un número ingresado por el usuario.
- Busque e imprima aquellos números en un rango indicado por el usuario.
- Imprima a suma de dichos números.

**Formato de input**

Un número entero **A**, que representa el límite inferior del rango.
Un número entero **B**, que representa el límite superior del rango.
Un número entero **div** que representa el número divisor.

**Restricciones**
-  **A** < **B**
-  10⁻⁹ <= **A**,**B** <=10⁹
-  **A** <= **div** <= B

**Formato de output**

```c++
Números entre <A> y <B>, divisibles por <div>: 
<lista de números divisibles por div>
La suma es: <suma de div>
```


## Ejemplo
```c++
Ingrese límite inferior: 100
Ingrese límite superior: 200
Ingrese divisor: 9
Números entre 100 y 200, divisibles por 9:
108 117 126 135 144 153 162 171 180 189 198
La suma es: 1683
```

%%
```c++
#include <iostream>
using namespace std;

int main(){

int A, B, div;
cout << "Ingrese límite inferior: ";
cin >> A;
cout << "Ingrese límite superior: ";
cin >> B;
cout << "Ingrese divisor: ";
cin >> div;

int suma = 0;
for (int i = A; i < B; i++){
	if (i % div == 0){
		cout << " " << i;
		suma += i;
	}
}
cout << "\n La suma es: " << suma << endl;

}
```
%%