## swap()
> [!important] Definición
> Swap permite intercambiar el valor de dos variables.

```c++
#include <iostream>
using namespace std;

int main(){
	int a = 90;
	int b = -30;
	cout << "Valor de a antes: " << a << endl;

	cout << "Valor de a antes: " << b << endl;

	// intercambia los valores de a y b
	swap(a, b);
	cout << "Valor de a después: " << a << endl;

	cout << "Valor de b después: " << b << endl;

	return 0;
}
```

## pow()
> [!important] Definición
> pow() permite calcular la potencia, dado una base y un exponente.

```c++
#include <iostream>
#include<iomanip>
#include <math.h>
using namespace std;

int main()
{
	double a = 4.2, b = 6.3;

	double potencia = pow(x, y);
	// Imprimir el resultado con hasta dos decimales.
	cout << fixed << setprecision(2) << potencia << endl;

	return 0;
}

```

## min() y max()
>[!important] Definición
> Permite determinar el número menor y mayor de dos variables, respectivamente.

```c++
#include <algorithm>
#include <iostream>
using namespace std;

int main()
{
	int c = 5;
	int d = 7;
	cout << "el menor es: " << min(c, d) <<endl;
	cout << "el mayor es: " << max(c, d) <<endl;
 	return 0;
}
```

## gcd()

> [!important] Definición
> gcd() permite obtener el máximo común divisor entre dos números.

```c++
#include <algorithm>
#include <iostream>
using namespace std;

int main()
{
	int a = 15, b = 90;
	int ans = __gcd(a, b);

	cout << "gcd(" << a << ", " << b << ") = " << ans << endl;
	return 0;
}

```

## floor() y ceil()
> [!important] Definición
> floor() redondea hacia abajo, mientras que ceil() redondea hacia arriba.

```c++
#include <cmath>
#include <iostream>
using namespace std;

int main(){
	cout << "Test de floor" << "\n";
	cout << floor(4.9) << "\n";
	cout << floor(-2.6) << "\n";
	cout << "Test de ceil" << "\n";
	cout << ceil(6.1) << "\n";
	cout << ceil(-5.5) << "\n";

	return 0;
}

```