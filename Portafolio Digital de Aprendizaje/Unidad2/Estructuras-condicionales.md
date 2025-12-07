# ⚙️ Estructuras Condicionales

Las estructuras condicionales son esos giros inesperados del guion en un programa: permiten que el código elija qué hacer según se cumpla o no una condición. Como un semáforo que decide si deja pasar o detener, evitan errores obvios (como dividir entre cero) y le dan al software la capacidad de reaccionar con algo parecido al sentido común.  
Las estructuras condicionales se clasifican en 3 tipos principales: 

- **Condicional simple:** Un bloque de sentencias basado en una condición.  
- **Condicional doble:** Dos cursos de acción diferentes según una condición.  
- **Condicional múltiple:** Diferentes casos posibles para una condición.

---

## 🔹 Estructura Condicional Simple

Es una estructura de programación que evalúa una condición. Si esta es verdadera, se ejecutará el bloque de código que se encuentre dentro; si es falsa, la sentencia se ignora y el programa continúa con la siguiente instrucción.

📋 **Ejemplo:**  
> En el siguiente ejemplo el usuario debe ingresar un número entero como nota de promedio, y el algoritmo determina si está aprobado o no en base a su nota, si esta es mayor o menor que 7.

### 💡 Algoritmo en Diagrama de Flujo  
Imagen 6: Diagrama de flujo de "Algoritmo Promedio"

<img width="728" height="897" alt="image" src="https://github.com/user-attachments/assets/987bf727-4519-4102-a598-b6e071f50167" />

### 💻 Algoritmo en lenguaje C  
> En C se implementa mediante la sentencia **if**.

```
#include<stdio.h>

int main(){
    int n;
    printf("Ingrese la nota de su promedio: \n");
    scanf("%i", &n);

    if(n >= 7){
      printf("Usted ha aprobado\n");
    }
    printf("Evaluacion finalizada\n");

    return 0;

}
```
▶️ **Ejecución en C**

```
[matias@cachyos C]$ gcc ejercisioPromedio.c -o ejercisioPromedio
[matias@cachyos C]$ ./ejercisioPromedio
Ingrese la nota de su promedio: 
8
Usted ha aprobado
Evaluacion finalizada
```

---


## 🔸 Estructura Condicional Doble

Su característica principal es que permite elegir entre dos cursos de acción diferentes, dependiendo del valor de verdad de una expresión lógica. Si la condición es verdadera, se ejecuta un bloque de código; si es falsa, se ejecuta un segundo bloque.

📋 **Ejemplo:**  
> En el siguiente ejemplo se observa el mismo problema anterior, pero esta vez usando un condicional doble.

### 💡 Algoritmo en Diagrama de Flujo  
Imagen 7: Diagrama de flujo de "Algoritmo Promedio2"

<img width="764" height="915" alt="image" src="https://github.com/user-attachments/assets/43e92dc4-3406-41d1-ab3d-af584c4b6701" />

### 💻 Algoritmo en lenguaje C  
> En C se implementa con la estructura **if...else**.

```
#include<stdio.h>

int main(){
    float n;
    printf("Ingrese la nota de su promedio: \n");
    scanf("%f", &n);

    if(n >= 7){
        printf("Usted a aprobado\n");
    }else{
        printf("Usted a reprobado\n");
    }
    printf("Evaluacion finalizada\n");

    return 0;

}
```
▶️ **Ejecución en C**

```
[matias@cachyos C]$ gcc ejercisioPromedio.c -o ejercisioPromedio
[matias@cachyos C]$ ./ejercisioPromedio
Ingrese la nota de su promedio: 
5
Usted a reprobado
Evaluacion finalizada
```

---


---

## 🔻 Estructura Condicional Múltiple

El condicional múltiple funciona como un pequeño portero lógico: recibe un valor, lo compara con varias opciones posibles y ejecuta solo la acción que coincida. En C se escribe con la sentencia **switch**, siempre basada en números o caracteres, y únicamente comprobando si algo es igual a algo.  
Si nada encaja aparece el **default**, la “salida de emergencia” que asegura que el programa siempre sepa qué hacer.

📋 **Ejemplo:**  
> En el siguiente ejemplo se observa el mismo problema anterior, pero esta vez usando un condicional múltiple.

### 💡 Algoritmo en Diagrama de Flujo  
Imagen 8: Diagrama de flujo de "Algoritmo Promedio3"

<img width="1853" height="561" alt="image" src="https://github.com/user-attachments/assets/df6b25ac-9bef-4d8a-a1c9-0b17004af439" />

### 💻 Algoritmo en lenguaje C  
> En C se implementa con la sentencia **switch**.

```
#include<stdio.h>

int main(){
    int n;
    printf("Ingrese la nota de su promedio: \n");
    scanf("%i", &n);
    switch(n) {
        case 7:
            printf("aprobado\n");
            break;
        case 8:
            printf("aprobado\n");
            break;
        case 9:
            printf("aprobado\n");
            break;
        case 10:
            printf("aprobado\n");
            break;
        case 0:
            printf("reprobado\n");
            break;
        case 1:
            printf("reprobado\n");
            break;
        case 2:
            printf("reprobado\n");
            break;
        case 3:
            printf("reprobado\n");
            break;
        case 4:
            printf("reprobado\n");
            break;
        case 5:
            printf("reprobado\n");
            break;
        case 6:
            printf("reprobado\n");
            break;
        default:
            printf("nota invalida\n");
            break;
    }

    return 0;

}
```
▶️ **Ejecución en C**

```
[matias@cachyos C]$ gcc ejercisioPromedio.c -o ejercisioPromedio
[matias@cachyos C]$ ./ejercisioPromedio
Ingrese la nota de su promedio: 
9
aprobado
```
---


---

## 🧩 Estructuras con Anidaciones

El término *anidamiento de estructuras condicionales* se refiere a la práctica de colocar una estructura condicional (como un **if**, **else if** o **else**) dentro de otra.  
Esto permite evaluar múltiples condiciones de manera sucesiva.  
Por este motivo, también se consideran como estructuras condicionales múltiples.

📋 **Ejemplo:**  
> En el siguiente ejemplo se observa el mismo problema anterior, pero esta vez usando una sentencia anidada.

### 💡 Algoritmo en Diagrama de Flujo  
Imagen 9: Diagrama de flujo de "Algoritmo Promedio4"

<img width="1373" height="900" alt="image" src="https://github.com/user-attachments/assets/b47748b0-cae2-413d-9aa7-a8dfd0b62b7e" />

### 💻 Algoritmo en lenguaje C

```
#include<stdio.h>

int main(){
    int n;
    printf("Ingrese la nota de su promedio: \n");
    scanf("%i", &n);

    if(n==10){
        printf("Excelente, aprobado\n");

    }else if(n >= 7){
        printf("Aprobado\n");
    }else if(n >= 5){
        printf("A recuperacion\n");
    }else {
        printf("Reprobado\n");
    }

    return 0;

}
```
▶️ **Ejecución en C**

```
[matias@cachyos C]$ gcc ejercisioPromedio.c -o ejercisioPromedio
[matias@cachyos C]$ ./ejercisioPromedio
Ingrese la nota de su promedio: 
6
A recuperacion
```

---


[⬅️ Volver a Contenidos de la Unidad](../Entrada/Contenidos.md)

