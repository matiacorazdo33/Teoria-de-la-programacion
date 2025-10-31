# ⚙️ Algoritmos, Pseudocódigo y Diagramas de Flujo  

---

## 🧠 Algoritmos  

Un **algoritmo** es un conjunto de pasos ordenados de forma lógica y finita, diseñados para resolver un problema o cumplir una tarea específica.  
Cada paso debe estar claramente definido, de modo que, al usar los mismos datos de entrada, siempre se obtengan los mismos resultados [1].  
Todo algoritmo cuenta con tres elementos esenciales:  

- **Entradas:** los datos o información inicial necesarios.  
- **Proceso:** las operaciones o transformaciones que se aplican.  
- **Salidas:** los resultados o soluciones obtenidas.
    



📋 **Ejemplo:**  
>En el siguiente ejemplo se puede observar un algoritmo escrito a modo de solución para encontrar en área de un triángulo, con datos que el propio usuario debe asignar.

📐 **Algoritmo para Calcular el Área de un Triángulo**
1. Inicio
2. Definir (o nombrar) tres variables: base, altura y area.

//Entrada

3. Solicitar al usuario que ingrese el valor de la base del triángulo.

4. Guardar el valor ingresado en la variable base.

5. Solicitar al usuario que ingrese el valor de la altura del triángulo.

6. Guardar el valor ingresado en la variable altura.

//Proceso

7. Calcular el área multiplicando la base por la altura y luego dividiendo el resultado entre 2.

   area = (base × altura) / 2

//Salida

8. Mostrar el valor calculado de area al usuario, indicando que es el área del triángulo.

9. Fin


---

## 💬 Pseudocódigo  

El **pseudocódigo** es una herramienta utilizada para expresar de manera clara y estructurada los pasos de un algoritmo, sin emplear aun un lenguaje de programación formal.  
Sirve como puente entre el lenguaje natural y los lenguajes de programación, ya que permite escribir instrucciones de forma comprensible, pero siguiendo una lógica cercana a la que se usa al programar.  
Su objetivo es ayudar a planificar la solución antes de escribir el código real, facilitando la comprensión del proceso.

Entre las herramientas para programar en pseudocódigo encontramos a **PSeInt**, el cual es un instrumento de software orientada a ayudar a quienes están dando sus primeros pasos en lo que se refiere a la programación. Su principal atractivo es la ventaja que representa a aquellos que están iniciando en su aprendizaje de la programación, dicha ventaja es gracias a que utiliza un lenguaje en pseudocódigo bastante simple y en español, lo que facilita al usuario comprender la lógica detrás de la elaboración de algoritmos[3].




📋 **Ejemplo:**  
>A continuación se observa el mismo algoritmo antes mencionado, sin embargo esta vez esta escrito en pseudocódigo en la plataforma ´PseInt, contando con las palabras clave e instrucciones apropiadas para hayar la solución al mismo problema.

```
Algoritmo triangulo
	//Variables
	Definir base, altura Como Entero;
	//Entrada
	Escribir "Ingrese base";
	Leer base;
	Escribir "Ingrese altura";
	Leer altura;
	//Proceso 
	area = (base * altura) / 2;
	//Salida
	Escribir "El área del triangulo es: ", area;
	
FinAlgoritmo
```

>Una vez ejecutado el programa, se abrirá una ventana la cual llevará a cabo las funciones para las que hayamos programado el algorítmo.

```
*** Ejecución Iniciada. ***
Ingrese base
> 10
Ingrese altura
> 8
El área del triangulo es: 40
*** Ejecución Finalizada. ***
```

---

## 🔄 Diagramas de Flujo  

El **diagrama de flujo** es una representación gráfica del algoritmo, donde cada acción o decisión se muestra mediante símbolos conectados por flechas que indican el orden de ejecución.  
Esta herramienta es fundamental en la etapa de diseño, ya que permite visualizar cómo fluye la información y cómo se ejecutan las instrucciones paso a paso.  
Junto con el pseudocódigo, facilita la comprensión del funcionamiento lógico de un programa antes de implementarlo en código [4].  

Imagen 1: Simbolos de un diagrama de flujo.

<img width="482" height="454" alt="image" src="https://github.com/user-attachments/assets/2a0f6af1-1223-4d1e-93a8-60c5d18213bc" />




📋 **Ejemplo:**  
>La siguiente imagen muestra el un ejemplo del mismo algoritmo de los problemas anteriores, representado en forma de diagrama de flujo haciendo uso de los simbolos y formas caracteristicas del mismo.

Imagen 2: Algoritmo "triangulo" en diagrama de flujo.

<img width="488" height="915" alt="image" src="https://github.com/user-attachments/assets/62a8616d-9fad-41be-b6c5-6950231a1548" />


---

🧮 **Pruebas de escritorio**
Las pruebas de escritorio componen una perte fundamenteal en la elaboración de in algoritmo ya que representan la comprobación para determinar si los datos obtenidos son los esperados. Consiste en realizar un seguimiento manual del algoritmo, haciendo uso de lapiz, papel y nuestra mente, simulando los datos de entrada para verificar que el comportamiento del algoritmo es el esperado.


📋 **Ejemplo:**  
>En la siguiente tabla se ejemplifica una prueba de escritorio en forma de tabla, correspondiente al mismo problema planteado por los ejemplos anteiores, verificando la operación con 3 casos diferentes para los datos de entrada.

Tabla 1: Prueba de escritorio del algoritmo "triangulo".
| **Entrada** |        | **Proceso**     | **Salida** |
|:------------:|:------:|:----------------|:-----------:|
| **Base**     | **Altura** | *(base × altura) / 2* | *(Área)* |
| 10 | 8 | (10 × 8) / 2 | 40 |
| 3  | 6 | (3 × 6) / 2 | 9 |
| 22 | 15 | (22 × 15) / 2 | 165 |


[⬅️ Volver a Contenidos de la Unidad](../../Entrada/Contenidos.md)

