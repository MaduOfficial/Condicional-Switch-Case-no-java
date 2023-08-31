Condicional-Switch-Case-no-java

                                                                           Condicional Switch - Case


.COMANDO Switch - Case


                                                                             Comando Switch - Case

.Funciona como múltiplos If-Else


                                                                  fazer programa com 0 Condicional Switch - Case


fazer um programa em que entremos com o dia da semana de 1 a 7, se o usuário entrar no 1 imprime domingo se for 2 segunda e assim vai.

vamos usar o código Scanner

		Scanner scan = new Scanner (System
		
		System.out.println("Entre com um dia da semana (1-7):");
		
		int diaSemana = scan.nextInt();
		
		if (diaSemana == 1){
		System.out.println("Domingo");
	} else if (diaSemana == 2){
		System.out.println("Segunda");
	} else if (diaSemana == 3){
			System.out.println("terça");
	} else if (diaSemana == 4){
		System.out.println("Quarta");
	} else if (diaSemana == 5){
			System.out.println("Quinta");
	} else if (diaSemana == 6){
		System.out.println("Sexta");
	} else if (diaSemana == 7){
			System.out.println("Sábado");
	} else {
		System.out.println("Não é um dia da semana válido");
    }
  }
}

Vamos fazer o código gerar no console o dia das semanas que vamos digitando de 1 a 7, se digitarmos 9 ou qualquer outro número que não tem no dia da semana
vai dizer que o número não é válido > Não é um dia da semana válido.Se você quer que o código switch case funcione como o If Else é só colocar "break".

package com.madu.Condicional.Switch.Case;

import java.util.Scanner;

public class SwitchCase {

	public static void main(String[] args) {
		
		Scanner scan = new Scanner (System.in);
		
		System.out.println("Entre com um dia da semana (1-7):");
		
		int diaSemana = scan.nextInt();
		
		if (diaSemana == 1){
		System.out.println("Domingo");
	} else if (diaSemana == 2){
		System.out.println("Segunda");
	} else if (diaSemana == 3){
			System.out.println("terça");
	} else if (diaSemana == 4){
		System.out.println("Quarta");
	} else if (diaSemana == 5){
			System.out.println("Quinta");
	} else if (diaSemana == 6){
		System.out.println("Sexta");
	} else if (diaSemana == 7){
			System.out.println("Sábado");
	} else {
		System.out.println("Não é um dia da semana válido");
    }
		
		
	switch(diaSemana){
	case 1: System.out.println("Domingo"); break;
	case 2: System.out.println("Segunda"); break;
	case 3: System.out.println("Terça"); break;
	case 4: System.out.println("Quarta"); break;
	case 5: System.out.println("Quinta"); break;
	case 6: System.out.println("Sexta"); break;
	case 7: System.out.println("Sábado"); break;
	default: System.out.println("Não é um dia da semana válido");
	}
  }
}



EX3:O breack ele é como se fosse fechar os parênteses, se a gente não coloca o breack no código ele esecuta todos os comandos até ele achar o breack, mesmo
que esse comando não seja verdadeiro, exemplo se eu digitar 1 que é domingo ele vai digitar tudo domingo, segunda, quarta, quinta, sexta e sábado, ele
executa todo o bloco de código até achar um break.

package com.madu.Condicional.Switch.Case;

import java.util.Scanner;

public class SwitchCase {

	public static void main(String[] args) {
		
		Scanner scan = new Scanner (System.in);
		
		System.out.println("Entre com um dia da semana (1-7):");
		
		int diaSemana = scan.nextInt();
	
	switch(diaSemana){
	case 1: System.out.println("Domingo");
	case 2: System.out.println("Segunda");
	case 3: System.out.println("Terça");
	case 4: System.out.println("Quarta");
	case 5: System.out.println("Quinta");
	case 6: System.out.println("Sexta");
	case 7: System.out.println("Sábado"); break;
	default: System.out.println("Não é um dia da semana válido");
  }
 }
}

COM O COMANDO ACIMA SE A GENTE DIGITAR 1 VAI APARECER TODO O CÓDIGO DE DOMINDO A SÁBADO, SE ESCREVERMOS 3 VAI APARECER DE TERÇA A SÁBADO ATÉ O COMANDO BREACK.

eX:
Entre com um dia da semana (1-7):
3
Ter?a
Quarta
Quinta
Sexta
S?bado

                                IMPORTANTE

No if e no else if (diaSemana == 1){   else if (diaSemana == 2){ repare que dentro do código nós temos expressões, o resultado dessas expressões sempre vai
ser um booleano então é se um dia da semana é igual a 1, se o dia da semana é maior que 1, se o dia da semana é menor que 1, se o dia da semana é igual a 1 e
uma outra váriavel ou uma outra váriavel a gente sempre utiliza um expressão lógica útilizando operadores lógicos e relasionais cuja o resultado vai ser
sempre um booleano o resultado vai ser true ou false, no switch case é diferente.

                               Swithc JAVA>7

.Até java 7 a condição podia ser byte, short, int, char ou Enum

.Com java 7 o switch também aceita String

Dentro do switch a gente pode útilizar um byte, short, int, char ou Enum, o switch também aceita uma String.
