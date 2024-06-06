# cadastro-de-dados.C

#include <stdio.h>
#include <stdlib.h>

int main (){

        int opcao,opcao1,opcao2,opcao3,opcao4,quant;
        struct referencia{
            char nome0[100],nome1[100],nome2[100],nome3[100],nome4[100];
    }
CA[600];
CA[600];
CA[600];
CA[600];
CA[600];
CA[600];
CA[600];
        char nome5[100];

    system("cls");
    printf("Digite o seu nome: ");
    fflush(stdin);
    scanf("%[^\n]s",nome5);
    printf("Digite a senha da impresa: ");
    scanf("%d",&opcao3);

        switch(opcao3){
         case 123456:

            while(opcao!=6){
    while(opcao2!=1){
        system("color f0");
        system("cls");

            printf("---------------------------------------------------------------");
            printf("\t\t\t\tloja C&A\n");
            printf("---------------------------------------------------------------\n\n");
            printf("\t\t\tSeja Bem Vindo, Atendente %s\n",nome5);
            printf("_______________________________________________________________\n ");
            printf("1-Cadastrar\n ");
            printf("2-Exibir Dados\n ");
            printf("3-Alterar\n ");
            printf("4-Excluir\n ");
            printf("5-Informacoes do Sistema\n ");
            printf("6-Sair\n ");
            printf("---------------------------------------------------------------\n\n");
            printf("\nQual opcao voce deseja acesser? ");
            scanf("%d",&opcao);

    switch(opcao){
        case 1:
            system("cls");
            printf("\n\n Quantos cadastros voce deseja realizar? ");;
            scanf("%d",&quant);

        for(int i=1;i<=quant;i++){
            system("cls");
            printf("\n\n\t\t\t      INICIANDO CADASTRO %d\n",i);
            printf("\t\t\t      -----------------------\n\n");
            printf("\n Nome do comprador: ");
            fflush(stdin);
            scanf("%[^\n]s",CA [i].nome0);
            printf("\n Telefone do comprador: ");
            fflush(stdin);
            scanf("%[^\n]s",CA [i].nome1);
            printf("\n Marca do produto: ");
            fflush(stdin);
            scanf("%[^\n]s",CA [i].nome2);
            printf("\n Codigo do produto: ");
            fflush(stdin);
            scanf("%[^\n]s",CA [i].nome3);
            printf("\n Preco do produto: ");
            fflush(stdin);
            scanf("%[^\n]s",CA [i].nome4);
            printf("\n\n\t\t");
            system("pause");
            system("cls");
        }
        break;

        case 2:
            system("cls");

            for(int i=1;i<=quant;i++){
                system("cls");
                printf("\n\n\t\t\t      EXIBINDO CADASTRO %d\n",i);
                printf("\t\t\t      -----------------------\n\n");
                printf(" Nome do comprador : %s\n",CA [i].nome0);
                printf("\n Telefone do comprador : %s\n",CA [i].nome1);
                printf("\n marca do produto : %s\n",CA [i].nome2);
                printf("\n codigo do produto : %s\n",CA [i].nome3);
                printf("\n preco do produto : %s\n",CA [i].nome4);
                system("pause");
            }
                    break;

                    case 3:
                        system("cls");
                        for(int i=1;i<=quant;i++){
                            printf("\n\n\t\t\t      ALTERAR CADASTRO %d\n",i);
                            printf("\t\t\t      -----------------------\n\n");
                            printf("1- Nome do comprador");
                            printf("\n 2- Telefone do comprador");
                            printf("\n 3- Marca do produto");
                            printf("\n 4- codigo do produto");
                            printf("\n 5- preco do produto\n\n");
                            printf("Qual opcao voce deseja alterar? \n");
                            scanf("%d",&opcao1);

        switch(opcao1){
            case 1:
                for(int i=1;i<=quant;i++){
                    system("cls");
                    printf("\n\n CADASTRO %d\n",1);
                    printf("\n Alterar nome do comprador: ");
                    fflush(stdin);
                    scanf("%[^\n]s",CA [i].nome0);
                    printf("\n Novo nome do comprador: %s\n\n\t\t");
                    system("pause");
                }
                break;

            case 2:
                for(int i=1;i<=quant;i++){
                    system("cls");
                    printf("\n\n CADASTRO %d\n",1);
                    printf("\n Alterar telefone comprador: ");
                    fflush(stdin);
                    scanf("%[^\n]s",CA [i].nome1);
                    printf("\n Novo telefone do comprador: %s\n\n\t\t");
                    system("pause");
                }
                break;

            case 3:
                for(int i=1;i<=quant;i++){
                    system("cls");
                    printf("\n\n CADASTRO %d\n",1);
                    printf("\n Alterar marca do produto: ");
                    fflush(stdin);
                    scanf("%[^\n]s",CA [i].nome2);
                    printf("\n Nova marca do produto: %s\n\n\t\t");
                    system("pause");
                }
                break;

            case 4:
                for(int i=1;i<=quant;i++){
                    system("cls");
                    printf("\n\n CADASTRO %d\n",1);
                    printf("\n Alterar codigo do produto: ");
                    fflush(stdin);
                    scanf("%[^\n]s",CA [i].nome3);
                    printf("\n Nova codigo do produto: %s\n\n\t\t");
                    system("pause");
                }
                break;

             case 5:
                for(int i=1;i<=quant;i++){
                    system("cls");
                    printf("\n\n CADASTRO %d\n",1);
                    printf("\n Alterar preco do produto: ");
                    fflush(stdin);
                    scanf("%[^\n]s",CA [i].nome4);
                    printf("\n alterar preco do produto: %s\n\n\t\t");
                    system("pause");
                }
                break;
            }
        }
        break;

            case 4:
                system("cls");
                for(int i=1;i<=quant;i++){
                                    printf("\n\n\t\t\t      EXCLUIR CADASTRO\n");
                                    printf("\t\t\t      -------------------\n\n");
                                    printf("1- Nome do comprador");
                                    printf("\n 2- Telefone do comprador");
                                    printf("\n 3- Marca do produto");
                                    printf("\n 4- codigo do produto");
                                    printf("\n 5- preco do produto\n\n");
                                    printf("Qual opcao voce deseja alterar? \n");
                                    scanf("%d",&opcao4);

                    switch(opcao4){
                        case 1:
                            for(int i=1;i<=quant;i++){
                                system("cls");
                                memset(&CA [i].nome0,0,sizeof(CA [i].nome0));
                                printf("Nome do comprador excluido!\n\n");
                                system("pause");
                            }
                            break;

                        case 2:
                            for(int i=1;i<=quant;i++){
                                system("cls");
                                memset(&CA [i].nome1,0,sizeof(CA [i].nome0));
                                printf("telefone do comprador excluido!\n\n");
                                system("pause");
                            }
                            break;

                        case 3:
                            for(int i=1;i<=quant;i++){
                                system("cls");
                                memset(&CA [i].nome2,0,sizeof(CA [i].nome0));
                                printf("marca do produto excluido!\n\n");
                                system("pause");
                            }
                            break;

                        case 4:
                            for(int i=1;i<=quant;i++){
                                system("cls");
                                memset(&CA [i].nome3,0,sizeof(CA [i].nome0));
                                printf("codigo do produto excluido!\n\n");
                                system("pause");
                            }
                            break;

                        case 5:
                            for(int i=1;i<=quant;i++){
                                system("cls");
                                memset(&CA [i].nome4,0,sizeof(CA [i].nome0));
                                printf("preco do produto escluido!\n\n");
                                system("pause");
                            }
                            break;

                        case 6:
                            for(int i=1;i<=quant;i++){
                                memset(&CA[i].nome0,0,sizeof(CA[i].nome0));
                                memset(&CA[i].nome1,0,sizeof(CA[i].nome1));
                                memset(&CA[i].nome2,0,sizeof(CA[i].nome2));
                                memset(&CA[i].nome3,0,sizeof(CA[i].nome3));
                                memset(&CA[i].nome4,0,sizeof(CA[i].nome4));
                                printf("todos os dados foram excluidos\n\n");
                                system("pause");
                            }
                            break;
                    }
                }
                break;

            case 6:
                system("cls");
                printf("\n Voce realmente deseja sair do sistema da loja?\n\n");
                printf("1- S\n 2-N");
                printf("\n\n" );
                scanf("%d",&opcao2);

            switch(opcao2){
                case 1:
                    system("cls");
                    printf("\n\n Volte sempre!! \n\n\n\t\t");
                    system("pause");
                    return 0;
                    break;
            }
            }
            }
            break;
            }
        }

system("pause");
return 0;
}
