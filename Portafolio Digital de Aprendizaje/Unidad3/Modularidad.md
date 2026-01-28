# 🧩 Estructuras Repetitivas

La modularidad es un principio de programación que consiste en dividir un programa en partes más pequeñas e independientes, llamadas módulos o funciones, donde cada una cumple una tarea específica.
Este enfoque permite que el código sea más ordenado, fácil de entender, mantener y reutilizar, ya que cada módulo puede desarrollarse, probarse y modificarse sin afectar directamente al resto del programa.

En lenguajes como C, la modularidad se aplica principalmente mediante el uso de funciones, que ayudan a estructurar mejor el programa y reducir la repetición de código.
Las funciones en C pueden recibir datos a través de parámetros, ya sea por valor o por referencia.

---


## 🔻 Uso de funciones en C.

Una función es un bloque de código que realiza una tarea específica y puede ser reutilizado dentro de un programa.

Una función en C se compone de:

- **Tipo de retorno:** Indica el tipo de dato que devuelve la función (int, float, void, etc.).

- **Nombre de la función:** Identificador que se utiliza para llamarla.

- **Parámetros:** Datos que recibe la función (pueden ser ninguno).

- **Cuerpo:** Conjunto de instrucciones que ejecuta la función.

➡️ Tipos de funciones:

- Funciones con retorno (devuelven un valor).

- Funciones sin retorno (void).

- Funciones con parámetros.

- Funciones sin parámetros.

 


### 📋 Sintaxis general de una funcion en C:
```
tipo_de_retorno nombre_funcion(tipo_parametro parametro){
    // instrucciones
    return valor; // El valor que se retorna, solo si no es void
}

```

---


## 🔹 Paso de parametros por valor

En el paso por valor, la función recibe una copia del valor de la variable original.
Los cambios realizados dentro de la función no afectan a la variable original.

➡️ **Tipo:** Paso de parámetros por valor

➡️ **Se usa cuando:** No se necesita modificar la variable original.




📋 **Ejemplo:**  
> El siguiente programa muestra cómo una función recibe un valor y lo modifica internamente sin afectar la variable original.

### 💻 Algoritmo en C
```
#include <stdio.h>

void suma(int x){
    x = x + 2;
    printf("valor dentro de la funcion: %i\n", x);

}

int main(){
    int numero = 5;

    suma(numero);
    printf("valor fuera de la funcion: %i\n", numero);

    return 0;
}
```

▶️ **Ejecución en C**

```
[matias@cachyos C]$ gcc parametrosPorValor.c -o parametrosPorValor
[matias@cachyos C]$ ./parametrosPorValor
valor dentro de la funcion: 7
valor fuera de la funcion: 5
```


---

## 🔸 Paso de parámetros por referencia

En el paso por referencia, la función recibe la dirección de memoria de la variable usando punteros.
Los cambios realizados dentro de la función sí afectan a la variable original.

➡️ **Tipo:** Paso de parámetros por referencia

➡️ **Se usa cuando:** Es necesario modificar la variable original desde la función.



📋 Ejemplo:

En el siguiente ejemplo, la función modifica directamente el valor de la variable usando un puntero.


### 💻 Algoritmo en C
```
#include <stdio.h>

void incremento(int *x){
    *x = *x + 2;

}

int main(){
    int numero = 5;

    incremento(&numero);
    printf("valor final: %i\n", numero);

    return 0;
}
```

▶️ **Ejecución en C**

```
[matias@cachyos C]$ gcc parametrosPorReferencia.c -o parametrosPorReferencia
[matias@cachyos C]$ ./parametrosPorReferencia
valor final: 7
```




---

[⬅️ Volver a Contenidos de la Unidad](../Entrada/Contenidos.md)






