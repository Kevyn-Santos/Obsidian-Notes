#Matematica 

Os critérios de divisibilidade são técnicas para verificar se um número pode ser dividido exatamente pelos números de 2 à 11 principalmente:

2 -> São divisíveis por 2 os números pares(terminados em 0,2,4,6,8)
3 -> Um número é divisível por três quando a soma dos seus algarismos for divisível por três
	p.ex: 
	2587 -> 2+5+8+7 = 22 -> 2+2 = 4; 4 não é divisível por 3, portanto 2587 também não é.
	333 -> 3+3+3 = 9; 9 é divisível por 3, portanto 333 também é
4 -> Um número é divisível por 4 quando os dois últimos algarismos formarem um número divisível por 4
	25**87** -> 87; 87 não é divisível por 4, então 2587 também não é
	30**40** -> 40; 40 é divisível por 4, então 3040 também é
	OBS: Se os últimos algarismos forem 0 o numero também é divisível por 4, pois 0 é divisível por qualquer número com exceção dele
5 -> Um número é divisível por 5 quando o ultimo algarismo for 0 ou 5
	8495 -> como o ultimo algarismo é 5 então todo o número é divisível por 5
	2587 -> como o ultimo algarismo não é 5, o número não será divisível por 5
6 -> Um número é divisível por 6 quando ele é divisível por 2 e 3 ao mesmo tempo
	2587 -> Não é divisível por 2(pois termina em impar) e não é divisível por três(pois a soma dos algarismos não é divisível por 3), logo, não é divisível por 6
	3040 -> é divisível por 2(pois termina em 0) mas não é divisível por 3(pois a soma dos algarismos da 7), logo, ele não é divisível por 6
	1350 -> é divisível por 2(pois termina em 0) é divisível por 3(pois a soma dos algarismos da 9 e ele é divisível por 3), logo, o número é divisível por 6
7 -> A divisibilidade por 7 é uma série de passos, vou colocar duas formas de fazer:
	Nº de Exemplo: 78546921388
	**Explicação por vídeo:**
		1º agrupe o número em classes de três algarismos da direita para esquerda(388 / 213 / 469 / 785)
		2º divida cada número por 7 e armazene o resto
		3º Atribua para cada número, começando da esquerda, um sinal de negativo e positivo e opere os números
		4º Verifique se o ultimo resultado é divisível por 7, se for, então todo número é divisível por 7.
		Neste caso, após todo o passo a passo, 78546921388 não é divisível por 7.
	**Explicação por livro:**
		1º Divida o número em grupos de três algarismos.
		2º Numere cada grupo de um em diante começando da direita(os que forem numerados com números impares serão os grupos impares, e os que forem numerados com números pares serão os grupos pares.)
		3º Some entre si os números dos grupos impares e pares e armazene os resultados
		4º subtraia os resultados das somas dos grupos impares e pares.
		5º divida o resultado final por 7, se a divisão for exata então todo numero é divisível por 7
		Neste caso, o número 78546921388 também não é divisível por 7
8 -> Um número é divisível por 8 quando os três últimos algarismos formarem um número divisível por 8
	2**587** -> 587; 587 não é divisível por 8 então 2587 também não é
	30328 -> 328; 328 é divisível por 8, então 30328 também é
9 -> Um número é divisível por 9 quando a soma dos algarismos resultar em um número divisível por 9
	2587 -> 2+5+8+7 = 22; Como 22 não é divisível por 9 então 2587 também não é
	4901067 -> 4+9+0+1+0+6+7 = 27 -> 2+7 = 9; como 27(ou 9) é divisível por 9, então 4901067 também é
10 -> Um número é divisível por 10 quando o ultimo algarismo for zero
11 -> A divisão por 11 também é uma série de passos:
	78546921388
	**1º** faça uma soma alternada entre os algarismos e preserve o resultado(em outras palavras, some pulando um algarismo começando da primeira posição e depois da segunda posição. Em termos mais visuais, some primeiro, da esquerda para direita os números das casas: 1,3,5,7,9... e depois das casas 2,4,6,8..)
	**2º** faça a diferença entre os resultados e verifique se o novo resultado é divisível por 11
	Neste caso 78546921388 não é divisível por 11. E aplicando a regra 2587 também não é divisível por 11.

Uma dica geral para verificar critérios além de 11 é combinar outros critérios de divisibilidade igual é para o 6, por exemplo:
Um número seria divisível por 15 se ele for divisível por 3 e 5 ao mesmo tempo. 
Um número seria divisível por 18 se ele for divisível por 2 e nove ao mesmo tempo, etc.