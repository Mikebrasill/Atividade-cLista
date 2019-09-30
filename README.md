# Atividade-cLista
#include <stdlib.h>
int main()
{
    char texto1[100] = "Texto aleatorio para teste de c";
    int i = 0;
    for(i = 0; texto1[i] != '\0' && i<sizeof(texto1) ;i++){
    }
    printf("Possui %d caracteres", i);

    return 0;

}
#include <stdio.h>
#include <stdlib.h>
int main()
{

    char texto2[100];
    printf("Digite um texto de ate 100 caracteres: ");
    gets(texto2);
    int vogais = 0, i = 0;
    for(i =0; i<sizeof(texto2) && texto2[i] != '\0'; i++){
        if(texto2[i] == 'a' || texto2[i] == 'e' || texto2[i] == 'i' || texto2[i] == 'o' || texto2[i] == 'u' ){
            vogais++;
        }
        if(texto2[i] == 'A' || texto2[i] == 'E' || texto2[i] == 'I' || texto2[i] == 'O' || texto2[i] == 'U' ){
            vogais++;
        }
    }
    printf("\nO total de vogais digitadas no texto foi: %d", vogais);
    return 0;
}
#include <stdio.h>
#include <stdlib.h>
int main()
{

    char texto3[100];
    char texto4[100];
    int i = 0, txt3 = 0, txt4 =0;
    printf("Digite o primeiro texto de ate 100 caracteres: ");
    gets(texto3);
    printf("Digite o segunado texto de ate 100 caracteres: ");
    gets(texto4);

    for(txt3 = 0; texto3[txt3] != '\0' && txt3<sizeof(texto3) ;txt3++){
    }
    for(txt4 = 0; texto4[txt4] != '\0' && txt4<sizeof(texto4) ;txt4++){
    }
    for(i =0; i<100 && texto3[i] == texto4[i]; i++){
    }
    if(i == txt3+1 && i == txt4+1){
        printf("\n\nOs conteudos dos textos sao iguais");
    }
    return 0;
}
#include <stdio.h>
#include <stdlib.h>
int main()
{
    char texto5[100];
    char texto6[100];
    printf("Digite um texto de ate 100 caracteres: ");
    gets(texto5);
    int i = 0;
    for(i = 0; i<sizeof(texto5) && texto5[i] != '\0'; i++){
        texto6[i] = texto5[i];
    }
    printf("%s", texto6);
    return 0;

}
#include <stdio.h>
#include <stdlib.h>
int main()
{
    char *texto7 = "Aula de";
    char *texto8 = "tecnicas de desenvolvimento de algoritimos";
    char texto9[100];
    int i = 0, j = 0;
    for(i = 0; texto7[i] != '\0' && i<sizeof(texto9); i++){
        texto9[i] = texto7[i];
        }
    texto9[i] = ' ';
    i++;
    for(j = 0; texto8[j] != '\0'; j++, i++){
        texto9[i] =  texto8[j];
    }
    printf("%s", texto9);
    return 0;
}
