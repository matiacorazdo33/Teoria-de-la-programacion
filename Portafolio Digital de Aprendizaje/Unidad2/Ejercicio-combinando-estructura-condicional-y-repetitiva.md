# 🔄 Algoritmo Combinando Estructura Condicional y Repetitiva

---

Un algoritmo que combina **estructuras condicionales** y **estructuras repetitivas** permite tomar decisiones dentro de un ciclo que se repite varias veces.  
Esto es útil cuando un proceso debe ejecutarse repetidamente hasta cumplir una condición, y dentro del ciclo se deben analizar diferentes casos usando decisiones tipo *if…else*.

En este ejemplo, utilizamos un ciclo repetitivo para pedir notas y una estructura condicional para clasificarlas como:  
✔️ Excelente  
✔️ Aprobado  
✔️ Reprobado  
✔️ Inválida

---

## 📋 Ejemplo  
Un algoritmo que solicita repetidamente notas entre 0 y 10.  
El ciclo continúa **hasta que el usuario ingrese -1**, que actúa como *valor centinela* para detener el programa.

Por cada nota ingresada, el sistema debe mostrar:

- “Excelente” si es 10  
- “Aprobado” si es ≥ 7  
- “Reprobado” si es < 7  
- Y si está fuera del rango 0–10, mostrar error  

Este ejercicio combina:

- **Repetición:** pedir notas varias veces  
- **Condición:** clasificar cada nota  

---

## 🔁 Diagrama de flujo simplificado

<img width="1098" height="939" alt="image" src="https://github.com/user-attachments/assets/e4aa6148-66f3-455a-8c17-78cf7885776d" />

---

## 💻 Programa en Java

```
import java.util.Scanner;

public class Notas {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int nota = 0;

        System.out.println("Ingrese notas entre 0 y 10. Para salir ingrese -1.");

        while(nota != -1){
            System.out.print("Ingrese la nota: ");
            nota = sc.nextInt();

            if(nota == -1){
                System.out.println("Fin del programa.");
                break;
            } else if(nota == 10){
                System.out.println("Excelente");
            } else if(nota >= 7){
                System.out.println("Aprobado");
            } else if(nota >= 0){
                System.out.println("Reprobado");
            } else {
                System.out.println("Error: nota inválida");
            }
        }

        sc.close();
    }
}
```

---

## ▶️ Ejecución del programa

```
[matias@cachyos java]$ javac Notas.java
[matias@cachyos java]$ java Notas
Ingrese notas entre 0 y 10. Para salir ingrese -1.
Ingrese la nota: 10
Excelente
Ingrese la nota: 8
Aprobado
Ingrese la nota: 5
Reprobado
Ingrese la nota: -3
Error: nota inv?lida
Ingrese la nota: -1
Fin del programa.
```

---

## 🧮 Prueba de escritorio

| **Entrada** | **Condición evaluada** | **Salida**        |
|------------|-------------------------|-------------------|
| 10         | nota == 10              | Excelente         |
| 8          | nota ≥ 7                | Aprobado          |
| 5          | nota < 7                | Reprobado         |
| -3         | nota < 0 o > 10         | Error             |
| -1         | nota == -1              | Fin del programa  |

---

## 📌 Conclusión

Este ejercicio demuestra cómo combinar:

- Una **estructura repetitiva** (*while*) para solicitar datos múltiples veces.  
- Una **estructura condicional** (*if–else*) para clasificar cada nota.  
- Un **valor centinela** para finalizar el ciclo.  

Esto permite resolver problemas reales como el registro y evaluación de calificaciones, aplicando lógica estructurada y controlada.

---


[⬅️ Volver a Contenidos de la Unidad](../Entrada/Contenidos.md)





