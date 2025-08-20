### Introdução

É um método estatístico que analisa a relação de duas variáveis, uma chamada de dependente(Variável Y, ou resposta) e outra independente(uma variável X, ou explicativa). O objetivo é prever os valores da variável Y com base nos valores da variável X, e também averiguar como a variável Y se altera por conta de X.

O calculo de regressão Linear é feito por meio da seguinte fórmula:

![[Pasted image 20250731211906.png]]

onde:
Y -> Variável dependente
B0 ->  Valor esperado de Y para x=0
B1 -> Coeficiente de regressão(O quanto Y muda para cada mudança unitária de X)
X1 -> variável independente

O gráfico gerado por esta fórmula é uma reta chamada de 'linha de melhor ajuste'. Como para cada valor de X teremos um ponto diferente no gráfico a reta não consegue passar por todos, então os pontos por onde ela passa são os melhores resultados daquela simulação.

### Premissas de utilização de regressão linear simples

Os principais pontos a se observar na realização de uma regressão linear são os seguintes:

Linearidade -> As relações entre variáveis devem ser lineares
Independência de erros -> Os erros(resíduos) devem ser independentes entre si, ou seja, os resíduos de uma observação não podem influenciar outra e não podem ter padrões.
Homoscedasticidade -> Os erros(resíduos) devem possuir valor constante, independente do valor da variável X


