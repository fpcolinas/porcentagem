#include <stdio.h>
#include <stdlib.h>
#include <locale.h>

void aumento(float preco[],int tam)
{
int i;

 for(i=0;i<tam;i++)
{
if (preco[i]<50)
{
preco[i]=preco[i]*1.10;

 }
}
}

void imprime(float preco[],int tam)
{ int i;

 printf("\n\n \t\t >>>> Precos na função");
for(i=0;i<tam;i++)
{
printf("\n %.2f",preco[i]);
}
}

int main()
{
setlocale(LC_ALL,"");
float preco[10];
int i;

 for(i=0;i<10;i++)
{

 printf("\n ....................................................\n");
printf("\n\n Informe o valor do produto: \n");
printf("\n ....................................................\n\n");
scanf("%f", &preco[i]);
printf("\n\n");

 }

 aumento(preco,10);
imprime(preco,10);

 printf("\n\n \t\t >>>> Precos no main");
for(i=0;i<10;i++)
{
printf("\n %.2f",preco[i]);
}

return 0;
}
