1.
```js
programa {
	funcao inicio() {
		//Preciso digitar o nome
		// Ao digitar precisa 
		escreva("Carol")
	}
}
```

2. 
```js
programa {
	funcao inicio() {
		//Aqui vc pensa, o dado é inteiro ? Tem vírgula?
		inteiro idade
		escreva("Qual a idade ?")
		leia(idade)
		escreva("A idade é:", idade, " anos")
	}
}
```  
3.  media para aprovação

```js
programa {
	funcao inicio() {
		real nota1
		real nota2
		real media
		
		escreva("Escreva a primeira nota: ")
		leia(nota1)
		escreva("Escreva a segunda nota: ")
		leia(nota2)
		
		media = (nota1 + nota2) / 2
		
		escreva("Sua media foi: ", media)
		
		se(media >= 7){
		    escreva("Aprovação!")
		} senao{
		  escreva("Não teve aprovação!")
		}
	}
}
``` 

5. - Crie um algoritmo que leia dois valores diferentes e determine o maior.
```js
programa {
	funcao inicio() {
		inteiro numero1, numero2
		escreva("Digite um numero inteiro")
		leia(numero1)
		escreva("Digite um segundo numero inteiro")
		leia(numero2)
		
		se(numero1 > numero2){
		   escreva("Numero 1 é maior que número 2")

		}se(numero2 > numero1){
		   escreva("Numero 2 é maior que número 1")

		}senao{
		 escreva("Os dois números são iguais")

		}
		
	}
}
```
6-- Crie um algoritmo que ao digitar uma letra, verifica se ela é vogal, se for mostre a mensagem "A letra 'a' é uma vogal" ou se não for, escreva "A letra 'x' é uma consoante"

```js
programa  
{
	funcao inicio ()
	{ 	
		caracter letra
		
		escreva("Digite uma letra: ")
		leia(letra)

		// O Portugol diferencia caracteres minúsculos e maiúsculos, 
		// portanto é preciso verificar ambos os casos
		
		se 
		(
			letra == 'A' ou letra == 'E' ou letra == 'I' ou letra == 'O' ou letra == 'U' ou
			letra == 'a' ou letra == 'e' ou letra == 'i' ou letra == 'o' ou letra == 'u'			
		)
		{ 
			escreva("\nA letra '", letra, "' é uma vogal\n") 
		}
		senao
		{
			escreva("\nA letra '", letra, "' é uma consoante\n") 
		}		
	} 
}
``` 
7- Crie um algoritmo que peça a pessoa usuaria que informe dois números. Logo após, calcula e exibe:
```js

/* CLIQUE NO SINAL DE "+", À ESQUERDA, PARA EXIBIR A DESCRIÇÃO DO EXEMPLO
 *  
 * Copyright (C) 2014 - UNIVALI - Universidade do Vale do Itajaí
 * 
 * Este arquivo de código fonte é livre para utilização, cópia e/ou modificação
 * desde que este cabeçalho, contendo os direitos autorais e a descrição do programa, 
 * seja mantido.
 * 
 * Se tiver dificuldade em compreender este exemplo, acesse as vídeoaulas do Portugol 
 * Studio para auxiliá-lo:
 * 
 * https://www.youtube.com/watch?v=K02TnB3IGnQ&list=PLb9yvNDCid3jQAEbNoPHtPR0SWwmRSM-t
 * 
 * Descrição:
 * 
 * 	Este exemplo demonstra o uso do desvio condicional para criar uma mini 
 * 	calculadora. O programa pede ao usuário que informe dois números reais 
 * 	e a operação a ser executada entre estes números (soma, divisão, etc.).
 *   Por fim, é exibido o valor resultante da operação entre os dois números.
 * 
 * Autores:
 * 
 * 	Giordana Maria da Costa Valle
 * 	Carlos Alexandre Krueger
 * 	
 * Data: 01/06/2013
 */ 

programa
{
	funcao inicio()
	{
		caracter operador
		
		real resultado = 0.0, operando1, operando2

		escreva("Digite o primeiro número: ")
		leia(operando1)

		escreva("Digite o segundo número: ")
		leia(operando2)

		escreva("\n")
		
		escreva("Agora digite uma das operações ( + - * / ): ")
		leia(operador)

		/* Verifica qual foi a operação selecionada */
		
		se (operador == '+')
		{
			resultado = operando1 + operando2
			
		}
		senao  se(operador == '-')
		{
			resultado = operando1 - operando2
			
		}
		senao se(operador == '/')
		{
			resultado = operando1 / operando2
			
		}
		senao se(operador == '*')
		{
			resultado = operando1 * operando2
		}	

		limpa()
		
		escreva("Resultado:\n\n")
		escreva(operando1, " ", operador, " ", operando2, " = ", resultado)
		
		escreva("\n")
	}
}

