
# Ayudantía 1

## Presentación
## Reglas y normas
## Introducción
### Entornos de Desarrollo Integrado (IDE)
### [[Hello, World!|Hello, World!]]
### [[Input y Output]]
## Tipos de variables:
- Int ("%d"): 32 Bit integer  
- Long ("%ld"): 64 bit integer 
- Char ("%c"): Character type 
- Float ("%f"): 32 bit real value 
- Double ("%lf"): 64 bit real value 
### [[Rangos de datos]]
### Práctica:
Trabajas en una caja registradora. La caja te muestra el monto que debe pagar el cliente. El cliente te entregará un monto en efectivo para pagar su compra.

**Objetivo**

Imprime por consola la cantidad de billetes y monedas que debes entregar como vuelto.

**Formato de Input**

Una línea que contiene el monto **M** que debe pagar el cliente y, separado por un espacio, el dinero **D** con el que paga el cliente.

**Restricciones**
$$ 
\textbf{D}  >= \textbf{M} 
$$
$$
INT\_MIN < \textbf{D}, \textbf{M} <INT\_MAX 
$$
**Formato de Output**

Indicar el número de billetes y monedas a entregar de vuelto, cada tipo ($10.000, $5.000, $2.000, $1.000, $500 y $100) separados por un salto de línea.

%%
```c++
#include <iostream>
#include <math.h>
using namespace std;

int main(){
	int vuelto = 14300;
	int diezmil = vuelto/10000;
	cout << "Billetes de $10.000: " << diezmil << endl;
	vuelto = vuelto -(diezmil*10000);
	int cincomil = vuelto/5000;
	cout << "Billetes de $5.000: " << cincomil << endl;
	vuelto = vuelto - (cincomil*500);

	/*etc. */

return 0;

}
```
%%
