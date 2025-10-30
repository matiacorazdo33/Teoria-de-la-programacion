# 📏 Algoritmos con Estructuras Lineales o Secuenciales  

---

Un **algoritmo secuencial o lineal** se distingue porque todas sus instrucciones se ejecutan una tras otra, siguiendo un **orden continuo y sin saltos lógicos**.  
En este tipo de estructura, cada paso depende del anterior y conduce directamente al siguiente, formando un flujo simple y directo.  
Los algoritmos lineales emplean las operaciones básicas de control secuencial, como la **asignación de valores**, la **lectura de datos de entrada** y la **escritura o presentación de resultados**.  
Este tipo de estructura es ideal para resolver problemas donde el proceso no requiere condiciones ni repeticiones, sino una ejecución paso a paso.  

---

## 📋 Ejemplo 1:  
Un algoritmo que determina la **aceleración de un cuerpo** utilizando su velocidad inicial, velocidad final y el tiempo transcurrido. 

Se utiliza la fórmula:

a = (vf−vi) / 2

---
​
💡 **Algoritmo en PseInt**

A continuación se muestra el pseudocódigo desarrollado en PseInt.


```pseint
Algoritmo aceleracion
    // Definir variables
    Definir vi, vf, t, a Como Real;
    
    // Entrada
    Escribir "Ingrese el valor de la velocidad inicial en m/s: ";
    Leer vi;
    Escribir "Ingrese el valor de la velocidad final en m/s: ";
    Leer vf;
    Escribir "Ingrese el valor del tiempo en s: ";
    Leer t;
    
    // Proceso 
    a = (vf - vi) / t;
    
    // Salida
    Escribir "La aceleración del cuerpo es: ", a;
FinAlgoritmo
```

---
▶️ **Ejecución del algoritmo en PseInt.**

Antes de que el algoritmo sea ejecutado, el usuario debe ingresar los datos de entrada que el programa solicite. Durante la ejecución el programa calcula de manera automática la aceleración del cuerpo y muestra al usuario el resultado.

---

```
*** Ejecución Iniciada. ***
Ingrese el valor de la velocidad inicial en m/s:
> 5
Ingrese el valor de la velocidad final en m/s:
> 8
Ingrese el valor del tiempo en s:
> 3
La aceleración el cuerpo es: 1
*** Ejecución Finalizada. ***
```

---

💻 **Traducción al lenguaje C**
El algoritmo anterior se tradujo al lenguaje de programación C con el uso de Visual Studio Code.

```
#include<stdio.h>
#include<stdlib.h>

int main(){
float vi, vf, t, a;

printf("ingrese el valor de la velocidad inicial en m/s:\n ");
scanf("%f", &vi);
printf("ingrese el valor de la velocidad final en m/s:\n ");
scanf("%f", &vf);
printf("ingrese el valor del tiempo en segundos:\n ");
scanf("%f", &t);

a = (vf - vi) / t;

printf("la aceleracion del cuerpo es:%f\n", a);

return 0;

}
```

---

▶️ **Ejecución en C**
En la ejecucion del programa en C se obsrvaron los mismos resultados que en PseInt, verificando la correcta traducción del algoritmo.

```
PS C:\Users\miltonlab\Documents\matias> cd .\programasMatias\
PS C:\Users\miltonlab\Documents\matias\programasMatias> gcc aceleracion.c -o aceleracion      
PS C:\Users\miltonlab\Documents\matias\programasMatias> .\aceleracion.exe    
ingrese el valor de la velocidad inicial en m/s:
 5
ingrese el valor de la velocidad final en m/s:
 8
ingrese el valor del tiempo en segundos:
 3
la aceleracion del cuerpo es:1.000000
```
**NOTA:** Para ejecutar el algoritmo en C, primero se debe guardar el programa (Ctrl + s), despues se debe copilar usando el compilador GCC desde la línea de comandos con el comando "gcc nombre_archivo.c -o nombre_ejecutable". Finalmente se ejecuta el archivo con ayuda del comando "\nombre_archivo.exe".

---

## 📋 Ejemplo 2:

Un algoritmo que calcula la **distancia entre dos puntos** haciendo uso de sus coordenadas.

Se utiliza la fórmula:

d= ((X2-X1)^2+(Y2-Y1)^2)^ 1⁄2

---
​
💡 **Algoritmo en PseInt**

A continuación se muestra el pseudocódigo desarrollado en PseInt.



<img width="1231" height="965" alt="image" src="https://github.com/user-attachments/assets/8d1a639c-880f-47df-9fe5-38c349688441" />


[⬅️ Volver a Contenidos de la Unidad](../../Introduccion/Contenidos.md)



