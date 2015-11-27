#include <stdio.h>
 
int main() {
 
    int N,a=0,X,b=0, c; //variaveis de valores inteiros
     
     scanf("%d", &N); //leitura e atribuição de valor inteiro a variavel (N)
     
     if(1<= N&&N <= 100){ // DEFINIDO REGRA DE VALORES
    
     for( a=0; a<N; a++){
   
        scanf("%d", &X); // leitura e atribuição de valor inteiro a variavel (x)
      
        if (1 < X&&X <=10000000){ // DEFINIDO REGRA DE VALORES
     
     for (c=X-1; c>1; c--){ // analisar se x e divisivel por outros valores
     
     if(X%c==0)
     b++;
     }
     if (b!=0)
     
     printf("%d nao eh primo\n", X);
     
     else
     
     printf("%d eh primo\n", X);
     b=0; //zerar a variavel para repetir o processo novamente
     
     
        }
     }
     }
     
    
    return 0;
}
