Realice un programa que despliegue los separadores en miles de un **número entero** ingresado por teclado. Por ejemplo, usted ingresa el número 1234567890, y su programa debe imprimir por pantalla "$1.234.567.890".

Observe que **debe** incluir los caracteres "$" y "."

(El número no puede ser mayor a 100 caracteres).






```c++

#include <iostream>

using namespace std;
int main(){

    int digito, num, cont=0;
    int cadena[100]={0};

    cout << "Ingrese un número: ";
    cin >> num;

    while(num>0){
        digito = num%10;
        num = num/10;
        cadena[cont]=digito;
        cont++;
    }

    cout << "$";
    for(int i=cont-1; i>=0; i--){
        cout << cadena[i];
        if (i%3 == 0 && i!=0){
            cout <<".";
        }
    }

    return 0; 
}


```
