
SOMA DE FATORIAIS COM FOR EM-C



    #include <stdio.h>
    
    int main(){
    
    int num, i = 1, j = 1,  soma = 0, fatorial;
    
    do{
        printf("Veja o fatorial de um número!\n");
        printf("Digite um número: ");
        scanf("%d", &num);
    
        if(num < 0){
            printf("Digite um número positivo: ");
        scanf("%d", &num);
        }
    }while(num < 0);
    
    
     for(i = 1; i <= num; i++){
       
        fatorial = 1;
        
        for(j = i; j > 0; j--){
            fatorial = fatorial * j;
        
        }
        
        soma = soma + fatorial;
        printf("%d! = %d \n", i, fatorial);
    }
    printf("A soma dos fatoriais é: %d\n", soma);
     
   
    

    return 0;
    }
