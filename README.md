#include<stdio.h>

#include<string.h>

int main()

{

  int i,k;

  char pilla[100];

  char rev[100]="MyCaptian";

  FILE *fkk;

  fkk=fopen("hello.txt","w");

  fprintf(fkk,"%s",rev);

  fclose(fkk);

  fkk=fopen("hello.txt","r");

  fscanf(fkk,"%s",pilla);

  printf("%s \n",pilla);

  k=strlen(pilla);

  for(i=k-1;i>=0;i--)

  {

    printf("%c",pilla[i]);

  }

   

  fclose(fkk);

   

  FILE *fpp;

  fpp=fopen("bye.txt","w");

  fprintf(fpp,"%s",pilla);

  fclose(fpp);

   

   

    return 0;

}
