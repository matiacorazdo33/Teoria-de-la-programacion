# 📦 Arreglos (Arrays)

📘 ¿Qué es un arreglo?

Un arreglo es una estructura de datos que permite almacenar varios valores del mismo tipo bajo un mismo nombre, organizados en posiciones consecutivas de memoria.
Cada valor se accede mediante un índice, que normalmente comienza en 0.

Los arreglos son muy útiles cuando se trabaja con listas de datos como notas, edades, temperaturas, matrices o información tabular.

---
## 🔻 Tipos de arreglos.

En programación estructurada, especialmente en C, los arreglos se clasifican según la cantidad de dimensiones que poseen:

- Arreglos unidimensionales
- Arreglos bidimensionales
- Arreglos multidimencionales (con capas)

---
## 🔸 Arreglos en C.

Un arreglo se define indicando:

- **Tipo de dato** que almacenará.

- **Nombre** del arreglo.

- **Tamaño** (cantidad de elementos).

Cada elemento del arreglo se identifica mediante un índice, el cual empieza en 0.

---


## 🔹 Arreglo unidimensional (vector)

Un arreglo unidimensional es una lista de elementos almacenados en una sola fila.
Se utiliza comúnmente para guardar datos como notas, edades, precios, etc.


➡️ **Tipo:** Arreglo unidimensional

➡️ **Se usa cuando:** Se necesita almacenar varios valores de un mismo tipo en una sola dimensión.



📋 **Ejemplo:**  
> El siguiente programa almacena 5 números en un arreglo y luego los muestra en pantalla.

### 💻 Algoritmo en C
```
#include <stdio.h>

int main(){
    int numeros[5];
    int i;

    for (i=0 ; i<5 ; i++){

        printf("Ingrese un numero: ");
        scanf("%i", &numeros[i]);
    }

    printf("Los nuneros ingresados son: \n");
    for (i=0; i<5; i++){
        printf("%i\n", numeros[i]);
    }


    return 0;
}
```

▶️ **Ejecución en C**

```
[matias@cachyos C]$ gcc arregloUnidimensional.c -o arregloUnidimensional  
[matias@cachyos C]$ ./arregloUnidimensional  
Ingrese un numero: 1
Ingrese un numero: 2
Ingrese un numero: 3
Ingrese un numero: 4
Ingrese un numero: 5
Los nuneros ingresados son: 
1
2
3
4
5
```


---

## 🔸 Arreglo bidimensional (matriz)

Un arreglo bidimensional es una estructura de datos organizada en filas y columnas, similar a una tabla o matriz.

➡️ **Tipo:** Arreglo bidimensional

➡️ **Se usa cuando:** Se necesita representar datos en forma de filas y columnas (por ejemplo, tablas, matrices, notas de estudiantes).



📋 Ejemplo:

> El siguiente programa muestra los valores almacenados de una matriz de 3 filas y 4 columnas.


### 💻 Algoritmo en C
```
#include<stdio.h>
#include<stdlib.h>
#include<string.h>

int main(){
    int matriz[3][4];
    matriz[0][0]= 1;
    matriz[0][1]= 5;
    matriz[0][2]= 8;
    matriz[0][3]= 3;

    matriz[1][0]= 2;
    matriz[1][1]= 3;
    matriz[1][2]= 6;
    matriz[1][3]= 8;

    matriz[2][0]= 5;
    matriz[2][1]= 7;
    matriz[2][2]= 9;
    matriz[2][3]= 4;

    for(int i=0; i<3; i++){
        for(int o=0; o<4; o++){
            printf("fila %i columna %i = %i\n", i, o, matriz[i][o]);

        }
    }

    return 0;
}
```

▶️ **Ejecución en C**

```
[matias@cachyos C]$ gcc arreglos.c -o arreglos             
[matias@cachyos C]$ ./arreglos             
fila 0 columna 0 = 1
fila 0 columna 1 = 5
fila 0 columna 2 = 8
fila 0 columna 3 = 3
fila 1 columna 0 = 2
fila 1 columna 1 = 3
fila 1 columna 2 = 6
fila 1 columna 3 = 8
fila 2 columna 0 = 5
fila 2 columna 1 = 7
fila 2 columna 2 = 9
fila 2 columna 3 = 4
```

📝 **Nota**

- Los índices de un arreglo siempre comienzan en 0.

- En un arreglo de tamaño n, el último índice válido es n - 1.

- Acceder a una posición fuera del rango puede provocar errores en el programa.


---

[⬅️ Volver a Contenidos de la Unidad](../Entrada/Contenidos.md)


