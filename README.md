# ImprimirMaiorNumeroJava
Montei esse código no intuito de fazer com que o usuário digite 10 valores e ao final de tudo o código imprima o maior valor digitado.


package ExerciciosDeControle;

import java.util.Scanner;

public class ImprimirMaiorNumero {
	public static void main(String[] args) {
		Scanner entrada = new Scanner(System.in);
		double valor;
		double maiorValor = 0;
		for(int i = 0; i <= 10; i++){
			System.out.println("Informe o valor: ");
			valor = entrada.nextDouble();
			if(valor > maiorValor) {
				maiorValor = valor;
			}
		}
		System.out.println("Maior valor: " + maiorValor);
		entrada.close();
	}
}
