```c++
#include <iostream>
using namespace std;
int main() {
    int a;
    cin>> a;
    cout << a << endl;
    return 0; 
}
```

```c++
#include <cstdio>
using namespace std;
int main() {
    int a , b;
    scanf("%d %d", &a, &b);
    printf("%d %d", a, b);
    return 0; 
}
```
#### Ejercicio:
Lee dos números enteros desde la terminal e imprime su suma, multiplicación, división y módulo.
%%
```c++
#include <iostream>
using namespace std; 
int main() { 
int a, b, c;
float aux;
cin >> a >> b >> c;
aux = a+b+c; 
cout << aux; 
return 0;
} 
```
%%
#### Ejercicio:
 Dibuja e imprime un triángulo rectángulo por terminal.
%%
```c++
#include <iostream> 
using namespace std; 
int main(){  
cout << "        /|" << endl;
cout << "       / |" << endl;
cout << "      /  |" << endl;
cout << "     /   |" << endl;
cout << "    /    |" << endl; 
cout << "   /     |" << endl; 
cout << "  /      |" << endl;  
cout << " /       |" << endl;  
cout << "/________|" << endl; 
return 0;
  }
```
%%
