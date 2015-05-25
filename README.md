Desafio de lógica
============

Esta página contém as informações referentes ao desafio de lógica para desenvolvedores juniors / assistentes

### Código de honra

Ao realizar esse desafio, você se compromete a:

* Não consultar outras pessoas sobre estratégias e soluções para os problemas propostos
* Não consultar mecanismos de busca online e offline sobre estratégias e soluções para os problemas propostos

### Questões

1. Você tem 8 moedas e todas tem o mesmo peso exceto uma, que é um pouco mais pesada que as demais. Você também possui uma balança que permite pesar duas pilhas de moedas para descobrir qual é a mais pesada (ou de mesmo peso). Qual é o mínimo número de combinações para serem feitas para descobrir qual a moeda mais pesada?

![alt text] (https://raw.githubusercontent.com/gszsilva/desafio-logica-junior/master/t-moedas.png "Resposta Moedas")

R. Apenas 2 combinações são necessárias para se saber qual é a mais pesada.

2. Assuma um cubo semelhante ao do desenho abaixo, no entanto com 8 mini cubos em cada aresta. Se pintarmos todas as suas faces, quantos mini cubos terão pelo menos uma face pintada?

![alt text] (https://raw.githubusercontent.com/maplink/desafio-logica-junior/master/121016-4x4x4-cube-175w.gif "Cubo 4x4")

R. Cada aresta possui 8 mini cubos
    8 * 8 = 64 (quantidade total de mini cubos por face)
    64 * 6 = 384 (quantidade total de faces de mini cubos visíveis)
    16 (quantidade de faces por mini cubos repetidos)
    384 - 16 = 368 mini cubos terão pelo menos uma face pintada.



3. Dado um array de inteiros ordenados, como encontrar a posição de determinado valor?



3. Escreva um código para reverter uma string.

Implementado em Java

{

import java.util.Scanner;
import java.util.Stack;

public class InvString {
	
	public static void main(String[] args) {
		
		Scanner ler = new Scanner(System.in);
		
		System.out.println("Digite uma string");
		String txt = ler.next();
		
		Stack s = new Stack();
		
		for (char c : txt.toCharArray()) {
			s.push(c);
		}
		
		String inv = "";
		
		while (!s.isEmpty()) {
			inv += s.pop().toString();
		}
		
		System.out.println("String invertida: " + inv);		
	}
}

}

### Envio da solução

Você pode realizar a implementação dos código na linguagem de programação de sua preferência. Use sua criatividade! 

O compartilhamento do resultado produzido deve ser feito diretamente pelo GitHub. Para isso, faça um <a href="https://help.github.com/articles/fork-a-repo" target="_blank">fork</a> e nos envie sua versão com a devida implementação e incluindo seus nome completo.

Qualquer dúvida, você pode enviar um e-mail para rhti@maplink.com.br.

Bom desafio!

*Time Maplink*
