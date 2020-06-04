#include <stdio.h>
#include <locale.h>
//declaração de variaveis
int main () {
  setlocale(LC_ALL, "Portuguese");
 int categorias,valorf,parcelas; 
 float totalfinal,cont=0;float descont,totalpagar;
 char resposta,resposta2;
 printf("Mateus Ferreira Porto\n");
 printf("mateusfporto@hotmail.com.br");
 //categorias
 do
 {
  printf(" \n\n 1- Verdura\n 2- legumes\n 3- Carnes\n 4- Limpeza \n Qual tipo de produto deseja comprar?");
  scanf("%d",&categorias);
  if(categorias == 1)
  {
    printf("ALFACE: R$ 3.80 (2.0 un)\n");
    printf("COUVE: R$ 4.53 (3.0 un)\n");
    printf("Total Verduras:R$ 8.33 ");
    cont=8.33;
  } else {
    if(categorias == 2)
    {
      printf("Cenoura : R$ 3.50 (0.8 KG)\n");
      printf("Batata : R$ 4.70 (4.5 KG)\n");
      printf("Vagem : R$ 2.80 (0.5 KG)\n");
      printf("Total Legumes: R$ 11.00");
      cont = 11.00;
    }
    else
    {
      if(categorias == 3)
      {
        printf("Alcatra : R$ 24.90 (2.0 KG)\n");
        printf("Patinho : R$21.50 (3.5 KG)\n");
        printf("Total Carnes: R$ 46.4");
        cont= 46.4;
      } 
      else
      {
        if(categorias == 4)
        {
          printf("Veja : R$ 5.70 (2.0 UN)\n");
          printf("Bombril : R$1.80 (3.5 PCT)\n");
          printf("limpol : R$1.99 (3.0 UN)\n");
          printf("Total Limpeza : R$9.49");
          cont = 9.49;
        }  
      } 
    } 
  }
totalfinal += cont;
printf("\nVocê deseja outra categoria? S ou N\n");
scanf(" %c", &resposta);

//estrutura de repetição
}while(resposta == 'S'|| resposta =='s');
 printf("obrigado pela compra ;)\n");
 printf("Total da sua compra é R$ %.2f",totalfinal);

//fim da parte 1!!!!!

  printf ("\nDigite o valor do desconto (valor da porcentagem)\n");
  scanf ("%f", &descont);

  printf ("O valor do desconto e de: %0.2f por cento\n", descont);

  valorf = totalfinal - (descont/100 * totalfinal);

  printf ("O novo valor da mercadoria com desconto e R$: %0.2d", valorf);
 
  printf ("\nForma de pagamento : Avista ou Parcelado (A/P)\n");
  scanf(" %c", &resposta2);

    if(resposta2 == 'A' || resposta2 == 'a')
    {
      printf("%d",valorf);
    }
    else
    {
      printf("Quantas parcelas você quer: ");
      scanf("%d", &parcelas);
      totalpagar= totalfinal / parcelas;
      printf("%.2f", totalpagar);
    }
}
