**Objetivo**
Identifica si es que un caracter ingresado es una letra o no.

**Formato de input**
Un caracter llamado **ch**.

**Restricciones**
**ch** es tipo Char.

**Formato de output**
Si el caracter ingresado es una letra, imprime por consola " **ch** es una letra.". En caso contrario, imprime "**ch** no es una letra."

%%
```c++
#include <iostream>
using namespace std;
int main(){
	char ch;
	cout << "Ingresa el caracter que desea revisar : ";
	cin >> ch;
	if(ch>='a' && ch<='z'){
		cout << ch << " es una letra." << endl;
	}
	else if(ch>='A' && ch<='Z'){
		cout << ch << " es una letra" << endl;
	}
	else {
		cout << ch << " no es una letra." << endl;
	}
	return 0;
}
```
%%