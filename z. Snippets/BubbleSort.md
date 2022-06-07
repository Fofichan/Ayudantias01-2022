# Bubble Sort u Ordenamiento de la Burbuja

Algoritmo de ordenamiento que compara dos elementos adjacientes e intercambia su posición hasta que estén en el orden deseado.

Al igual que las burbujas de aire en el agua que ascienden hacia la superficie, cada elemento del arreglo se mueve hasta el final de éste en cada iteración. De ahí el nombre, *Bubble sort*.

## Funcionamiento de Bubble Sort
### 1ra iteración (Comparar e intercambiar)
1. Comenzando con la primera posición, comparar el primer y segundo elemento.
2. Si el primer elemento es mayor que el segundo elemento, intercambian posición.
3. Comparar el segundo y tercer elemento. Intercambiarlos si es que no están en orden.
4. Repetir pasos de 1 al 3 hasta el último elemento.
![](https://github.com/Fofichan/Ayu01-2022/blob/main/zz.%20Recursos/Pasted%20image%2020220607030509.png)

El mismo proceso se repite por las iteraciones restantes. Después de cada iteración el elemento más grande dentro de los elementos no ordenados es ubicado al final.

![](https://github.com/Fofichan/Ayu01-2022/blob/main/zz.%20Recursos/Pasted%20image%2020220607032024.png)

Por cada iteración, la comparación se realiza hasta el último elemento no ordenado.
![](https://github.com/Fofichan/Ayu01-2022/blob/main/zz.%20Recursos/Pasted%20image%2020220607031830.png)

El arreglo queda ordenado cuando todos los elementos son ubicados en su posición correcta.
![](https://github.com/Fofichan/Ayu01-2022/blob/main/zz.%20Recursos/Pasted%20image%2020220607032142.png)
## Implementación
```c++
#include <iostream>
using namespace std;

void bubbleSort(int array[], int size) {

  // loop to access each array element
  for (int step = 0; step < size; ++step) {
      
    // loop to compare array elements
    for (int i = 0; i < size - step; ++i) {

      // compare two adjacent elements
      // change > to < to sort in descending order
      if (array[i] > array[i + 1]) {

        // swapping elements if elements
        // are not in the intended order
        int temp = array[i];
        array[i] = array[i + 1];
        array[i + 1] = temp;
      }
    }
  }
}

// print array
void printArray(int array[], int size) {
  for (int i = 0; i < size; ++i) {
    cout << "  " << array[i];
  }
  cout << "\n";
}

int main() {
  int data[] = {-2, 45, 0, 11, -9};
  
  // find array's length
  int size = sizeof(data) / sizeof(data[0]);
  
  bubbleSort(data, size);
  
  cout << "Sorted Array in Ascending Order:\n";  
  printArray(data, size);
}
```

**Fuente**: https://www.programiz.com/dsa/bubble-sort
