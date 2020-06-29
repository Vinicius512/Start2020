# Start2020
Código em portugol
programa
{
	
	funcao inicio()
	{
		cadeia aparelho = ""
		inteiro watts = 0, horas = 0, kilowatt = 00,consumo = 0, contafinal, sair = 0, mes = 30
		logico continuar = verdadeiro

		enquanto(aparelho !="SAIR" ){
		escreva("Qual o seu aparelho: ")
		leia(aparelho)
		se (aparelho != "SAIR"){
		escreva("Quantas horas esse aparelho fica ligado por dia: ")
		leia(horas)
		escreva("Quantos watts ele gasta por Hora: ")
		leia(watts)
		
	
		consumo = consumo + (horas*watts)
			
		}
			
			

		
		
	   }
	               contafinal = mes*consumo
	                kilowatt = contafinal/1000
			
	      escreva("Total de Kilowatt no mês gasto é: ", kilowatt)
	}
}
