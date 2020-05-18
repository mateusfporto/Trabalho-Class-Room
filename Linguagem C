#include<stdio.h>
int main (void){ 
float valori, descont, valorf;

  printf ("Didite o valor do produto\n");
  scanf ("%f", &valori);
  printf ("Digite o valor do desconto (valor da porcentagem)\n");
  scanf ("%f", &descont);

  printf ("O valor do desconto e de: %.2f por cento", descont);

  valorf = valori - (descont/100 * valori);
  printf ("\n\n");
  printf ("O novo valor da mercadoria com desconto e R$: %2.f", valorf);
 
    float x=0, y=0, total=0;
    int op=0;
    do{ 
       printf("\n\t1 - SOMA\n\t2 - SUBTRACAO\n\t3 - MULTIPLICACAO\n\t4 - DIVISAO");
       scanf("%i", &op);
       printf("\n Primeiro numero: ");
       scanf("%f", &x);
       printf("\n Segundo numero: ");
       scanf("%f", &y);
       switch(op){
           case 1:
               total = x+y; 
               break;
           case 2:
               total = x-y;
               break;
           case 3:
               total = x*y;
               break;
           case 4:
               total = x/y;
               break;
           default:
           printf("Digite um numero valido\n");
           break;
       }
       printf("\n\t o total e: %0.2f", total);
       printf("\n Digite 1 para continuar: ");
       scanf("%i", &op);
     }while(op==1);
  return 0;
}
