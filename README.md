# Atividade-11
#include <stdio.h>
#include <stdlib.h>
#include <Windows.h>
#include <locale.h>

char nome1, nome2, nome3, nome4;
double nota1_1, nota1_2, nota1_3, nota1_4;
double nota2_1, nota2_2, nota2_3, nota2_4;
double nota3_1, nota3_2, nota3_3, nota3_4;
double nota4_1, nota4_2, nota4_3, nota4_4;
 

void cadastro_notas() {
	system("cls");
	printf("Cadastro de Notas/Alunos\n");
	
	
	
	system("pause");	
	return;
}
void alteracao_notas() {
	system("cls");
	printf("Alteração de Notas/Alunos\n");
	
	
	
	system("pause");	
	return;
}

int main() {	
	setlocale(LC_ALL,"");
	int opcao=0;
	printf("Carregando o sistema... aguarde");
	Sleep(500);

	while ((opcao != 1) && (opcao !=2) && (opcao != 3)) {		
		// opcoes do menu
		system("cls");
		printf("Bem vindo ao meu sistema\n\n");
		printf("Menu\n");
		printf("----\n");
		printf("1-Cadastro de Notas/Alunos\n");
		printf("2-Alteracao de Notas/Alunos\n");
		printf("3-Sair\n");
		printf("Opção: ");
		scanf("%i",&opcao);
		// verificando as opcoes
		if (opcao == 1) {
			cadastro_notas();
			opcao = 0;
		} else {
			if (opcao == 2) {
				alteracao_notas();
				opcao = 0;
			} else {
				if (opcao == 3) {
					exit;
				}
			}
		}
	}
	
	return 0;
}
