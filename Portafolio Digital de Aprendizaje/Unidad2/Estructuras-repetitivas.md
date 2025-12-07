# 🔁 Estructuras Repetitivas

Las estructuras repetitivas permiten ejecutar un conjunto de instrucciones varias veces sin tener que escribirlas repetidamente. Son esenciales para automatizar tareas, reducir código y crear programas más eficientes.

En programación, los bucles se clasifican según **cómo** y **cuándo** evalúan su condición de repetición.  
Aquí los clasificamos por sus **tres estructuras principales: while, do-while y for**.

---

## 🔹 Ciclo `while` — *Bucle de condición previa*

El ciclo **while** evalúa una condición **antes** de ejecutar las instrucciones del bucle. Mientras la condición sea verdadera, el bloque se repetirá.

➡️ **Tipo:** Bucle controlado por condición  
➡️ **Se usa cuando:** No sabes cuántas veces se repetirá; depende de una condición.

📋 **Ejemplo:**  
> El siguiente elgoritmo pide un número N al usuario y muestra los números del 1 al N.

### 💡 Algoritmo en Diagrama de Flujo  
Imagen 10: Diagrama de "Algoritmo bucle" 


<img width="501" height="919" alt="image" src="https://github.com/user-attachments/assets/0f723528-c564-4beb-8717-2dae04a79392" />


### 💻 Algoritmo en C
```
#include<stdio.h>
int main(){
    int n, i=1;
    printf("Ingrese un numero: ");
    scanf("%i", &n);

    while(i<=n){
        printf("%i\n", i);
        i= i + 1;
    }

    return 0;

}
```

▶️ **Ejecución en C**

```
[matias@cachyos C]$ gcc ejercisioBucle.c -o ejercisioBucle
[matias@cachyos C]$ ./ejercisioBucle
Ingrese un numero: 4
1
2
3
4
```


---

## 🔸 Ciclo `do…while` — *Bucle de condición posterior *

El ciclo **do…while** ejecuta las instrucciones **al menos una vez** antes de preguntar si debe repetirse. Primero ejecuta, luego evalúa.

➡️ **Tipo:** Bucle controlado por condición  
➡️ **Se usa cuando:** Necesitas que el bloque se ejecute mínimo una vez (por ejemplo, validar entradas).

📋 **Ejemplo:**  
> En el siguiente ejemplo se observa el mismo problema anterior, pero esta vez usando el bucle **do...while**.

### 💡 Algoritmo en Diagrama de Flujo  
Imagen 11: Diagrama de "Algoritmo bucle2" 

<img width="660" height="921" alt="image" src="https://github.com/user-attachments/assets/b913e177-feb6-4c01-9e5f-1f8b5f5921c6" />


### 💻 Algoritmo en C
```
#include<stdio.h>
int main(){
    int n, i=1;
    printf("Ingrese un numero: ");
    scanf("%i", &n);

    do{
        printf("%i\n", i);
        i++;

    }while(i <= n);

    return 0;

}
```

▶️ **Ejecución en C**

```
[matias@cachyos C]$ gcc ejercisioBucle.c -o ejercisioBucle
[matias@cachyos C]$ ./ejercisioBucle
Ingrese un numero: 4
1
2
3
4
```


---

## 🔻 Ciclo `for` — *Bucle controlado por contador*

El ciclo **for** ejecuta un bloque un número **determinado** de veces. Es ideal cuando conoces cuántas repeticiones necesitas y quieres controlar:

- Valor inicial  
- Condición de fin  
- Incremento o decremento  

➡️ **Tipo:** Bucle controlado por contador  
➡️ **Se usa cuando:** El número de iteraciones está definido desde el inicio.

📋 **Ejemplo:**  
> En el siguiente ejemplo se observa el mismo problema anterior, pero esta vez usando el bucle **for**.

### 💡 Algoritmo en Diagrama de Flujo  
Imagen 12: Diagrama de "Algoritmo bucle3" 

<img width="765" height="910" alt="image" src="https://github.com/user-attachments/assets/e20104c1-a13c-4688-ad13-1fb0775218c9" />


### 💻 Algoritmo en C
```
#include<stdio.h>
int main(){
    int n, i;
    printf("Ingrese un numero: ");
    scanf("%i", &n);

    for (i=1; i<=n; i++){
        printf("%i\n", i);

    }

    return 0;

}
```

▶️ **Ejecución en C**

```
[matias@cachyos C]$ gcc ejercisioBucle.c -o ejercisioBucle
[matias@cachyos C]$ ./ejercisioBucle
Ingrese un numero: 4
1
2
3
4
```

---

[⬅️ Volver a Contenidos de la Unidad](../Entrada/Contenidos.md)






