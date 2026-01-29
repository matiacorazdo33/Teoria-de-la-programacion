```
#include <stdio.h>

void calcularValorCliente(float *total){
  int consola;
  int horas;
  float valorCliente;

   printf("Ingrese el numero de la consola en la que desea jugar(1=PlayStation, 2=Xbox, 3=Nintendo): ");
   scanf("%i", &consola);

    while(consola<1 || consola>3){
      printf("Ingrese un numero valido(1=PlayStation, 2=Xbox, 3=Nintendo): ");
      scanf("%i", &consola);
    }
    switch(consola){
      case 1:
        printf("Ingrese el numero de horas que desea jugar: ");
        scanf("%i", &horas);
        valorCliente = horas * 2.5;
        break;
      case 2:
        printf("Ingrese el numero de horas que desea jugar: "); 
        scanf("%i", &horas);
        valorCliente = horas * 2;
        break;
      case 3:
        printf("Ingrese el numero de horas que desea jugar: ");
        scanf("%i", &horas);
        valorCliente = horas * 1.5;
        break;
      default:
       printf("Numero invalido");

    }
    printf("El valor a pagar es de %f\n", valorCliente);

    *total = *total + valorCliente;

}


float calcularValorRecaudado(int clientes){
  int nc = clientes;
  int i;
  float total;

  for(i=0; i<nc; i++){
    printf("CLIENTE %i\n", i);
    calcularValorCliente(&total);
      
    }
printf("El valor recaudado es de %f", total);
  
  
}



int main() {
  int clientes;
  
  printf("Ingrese el numero de clientes\n");
  scanf("%i", &clientes);

  calcularValorRecaudado(clientes);

  
  return 0;
}

```
---
[⬅️ Volver a Contenidos de la Unidad](../Entrada/Contenidos.md)
