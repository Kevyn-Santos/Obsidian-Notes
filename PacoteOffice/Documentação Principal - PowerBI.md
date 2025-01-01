# Power BI

## **POWER QUERY**

O Power Query é uma ferramenta do Power BI que permite o tratamento dos dados antes destes serem importados para um uso mais complexo, é esta ferramenta que permite a exclusão ou inclusão de colunas e linhas, a mudança dos tipos de dados, a mesclagem de tabelas ou colunas, dentre outras coisas. Em suma, esta é a ferramenta que permitirá um tratamento inicial e fundamental dos dados que serão utilizados ao longo do relatório.


### Importação de dados

O Power BI permite que sejam importados dados de vários locais diferentes, como paginas da web, Bancos de dados, arquivos JSON, XML ou PDF, entre outros, mas o principal é a importação por meio de arquivos do Excel. Assim que um relatório novo for aberto será mostrado alguns botões para a importação dos dados, mas há outros locais para clicar caso queira mais opções, vamos passar por cada uma:

*Importação na pagina inicial*
![[Pasted image 20241225135624.png]]

*importação no cabeçalho*
![[Pasted image 20241225135713.png]] ![[Pasted image 20241225135845.png]]

Caso seja clicado da opção "Obter dados de outra fonte" ou "Obter dados"> "mais"

*mais fontes de dados*
 ![[Pasted image 20241225135905.png]]

Para os dados que vem de arquivos(Excel, CSV, PDF, etc.) será necessário indicar onde ele esta em seu computador, já para dados que vem de um banco de dados, é necessário fazer a conexão com o banco.

### Guia Transformar e Guia Adicionar coluna

Há duas guias principais no Power Query para o tratamento de dados, estão são as guias "Transformar" e a guia "Adicionar coluna", em termos gerais, elas fazem a mesma coisa porem a primeira modifica a coluna selecionada, substituindo seus valores, enquanto a segunda cria uma nova coluna e adiciona a modificação nela, nos próximos tópicos serão especificados os tipos de transformações que podem ser feitas dependendo do tipo de dado, e ficará mais clara esta distinção das modificações. 

Mas antes de passar para as tratativas diferentes de dados é bom falar da divisão entre estas duas guias. Apesar de ambas as guias fazerem a mesma coisa mas de formas diferentes a divisão entre elas muda um pouco, por exemplo, na guia "transformar" temos um campo especifico para transformações em toda tabela, outro para as transformações apenas em colunas, e outros para transformações de texto, números e datas.

Isso difere um pouco da guia "Adicionar colunas", pois nela temos o campo apenas para a adição de colunas, e outros para o tratamento de textos, números e datas. Sendo assim, a principal diferença na organização dos campos é que, enquanto na primeira guia podemos modificar a tabela toda, na segunda estamos limitados apenas a adição de colunas.

*Guia Transformar*
![[Pasted image 20241225134633.png]]

*Guia Adicionar Colunas*
![[Pasted image 20241225134738.png]]
### Transformar Dados – Texto

Transformar: Altera os valores da coluna original nela mesma

Adicionar Coluna: Altera os valores da coluna original, criando uma nova coluna com as alterações no final.

Extrair: extrai valores de uma coluna, utilizando algum delimitador ou regra.

Dividir valores: separa os valores de uma coluna em outras, utilizando algum delimitador ou regra.

### Transformar Dados – Numero

OBS: Alguns caracteres especiais não aparecem na parte de transformação de dados, eles aparecerão na parte do relatório

Numero decimal Fixo - Travado em duas casas decimais, é a formatação em moeda

Estatística – Transformar e Adicionar coluna:  
  
Transformar – Substitui toda a tabela pela estatística desejada da coluna

Adicionar coluna – é necessária mais de uma coluna, adiciona a estatística desejada destas colunas como uma nova coluna no final.

### Transformar Dados – Data

O calculo de idade vem no formato de hora, portanto é necessário tratar o dado de maneira mais especifica, da seguinte forma:  
  
Formatar para data> Pedir o cálculo de idade (Em adicionar coluna)> formatar a nova coluna como numero inteiro> dividir o numero por 365> conferir se está tudo correto.

### Transformar dados – colunas condicionais

Cria uma nova coluna baseada em algumas condições estabelecidas (funciona apenas em “Adicionar nova coluna”). É como uma formatação condicional.

Para tratar erros que possuem valor: botão direito na coluna> Substituir erros> valor que o erro deveria possuir.

### Transformar dados – coluna de índice

A coluna de índice será a coluna com as chaves primárias da tabela.

Para criar uma coluna de índice: selecione “Coluna de índice” em “Adicionar Coluna”>   Selecione o valor de início da coluna de índice.

### Ferramentas de dados

Agrupar – resume as informações da tabela tendo com referencia uma ou mais colunas, este resumo pode ser várias operações como soma, contar linhas, dividir, etc. Então por exemplo, caso você deseje o total de receita por estabelecimento. Você irá agrupar todos os estabelecimentos e somar os valores associados, se você quiser o total de receita de estabelecimentos divididos por tipo, a ferramenta vai filtrar estes tipos e vai te retornar à somatória das receitas. Então esta ferramenta agrupa as informações iguais e resume os valores associados a ela em alguma operação.

Mesclar – Junta os valores de duas ou mais colunas em uma terceira coluna

 Intercalar tabelas - junta os valores de duas ou mais tabelas em uma terceira tabela. É necessário ter colunas com valores iguais, pois elas serão as “Chaves primarias” para a junção.

Append – adiciona linhas com informações de outras tabelas

## **RELAÇÕES**

### O que são relacionamentos

Relacionamento no PowerBi é como fazer um join em um banco de dados, você tem em uma tabela certas informações e quer verificar o correspondente delas em outra tabela, como você faz isso? Utilizando uma relação, assim você liga duas colunas iguais em ambas as tabelas e com isso você consegue procurar estas informações correspondentes. 

*Nota:* É mais importante o conteúdo das colunas do que seus nomes, pois é a partir do conteúdo das colunas que as informações serão puxadas. 

As relações servem para você encontrar informações em uma tabela utilizando parâmetros de outra tabela, além de serem de extrema importância na montagem do relatório, pois é a partir das relações que as informações serão apresentadas de maneira apropriada. Para isso existem dois tipos de relações, as diretas e as indiretas.

Relações diretas: É quando você une diretamente duas tabelas que contenham colunas semelhantes.

Relações indiretas: Ocorre quando você precisa relacionar duas tabelas porem elas não possuem colunas semelhantes, então é usada uma terceira tabela, que contenha informações semelhantes as duas, para fazer a relação entre elas. Ou seja, você precisa relacionar a tabela 1 e 3, porem elas não possuem colunas semelhantes para serem relacionadas, então você utiliza a tabela 2, que contém informações tanto da tabela 1 quanto da tabela 3, para relacionar as tabelas necessárias, desta forma a tabela 1 e 3 estão relacionadas, porém, não diretamente.

  
### Base de informações(Fato) X Base de características(Dimensão):  
  
Uma base de informações é uma tabela que descreve várias informações sobre um tópico, então uma base de informações não retorna tentas características sobre seu conteúdo, não destrincha ele, não dá detalhes, ela simplesmente retorna várias informações diferentes sobre algo, por exemplo, uma tabela de clientes retorna várias informações diferentes sobre os clientes, porem não retorna os detalhes destas informações. Uma tabela de vendas me retorna diversas informações sobre as vendas que tive, mas não me retorna os detalhes sobre estas informações de vendas.

Para que você consiga os detalhes destas tabelas são necessárias as bases de características, elas são como tabelas auxiliares que retornam os detalhes das informações das bases de informações, então caso eu queria saber o nome de um produto vendido, pode ser que esta informação não esteja em uma tabela de vendas, mas vai estar em uma tabela de produtos, então basta eu buscar as informações na tabela de produtos. Caso eu queira saber o dia da semana que comecei um contrato com um cliente, pode ser que esta informação não esteja na tabela cliente, mas eu posso adquiri-la na tabela calendário, então basta eu procurar nesta ultima.

Uma observação importante: Tabelas fatos não possuem relações entre si, isso porque seus dados se repetem muito e com isso não há alguma informação exclusiva para cada iteração.
### Esquemas de relacionamentos - Esquema Estrela

O esquema estrela é uma das formas de se organizar uma serie de relações, ele pega uma tabela informação e a circunda com tabelas de caracterizas em uma formação que lembra uma estrela, por isso do nome, esta é a técnica mais útil para organização de tabelas. Mas, não são necessárias muitas tabelas para este padrão, três já são o bastante para formar relações esquema estrela.

Resumindo, um esquema estrela será uma forma de organizar relações, onde  as tabelas fato ficam no centro, sendo circundadas por tabelas de características que se relacionam com ela.


![[Pasted image 20241229192816.png]]

A imagem acima é um exemplo de esquema estrela, não esta muito na forma de uma estrela, mas ele fica neste padrão. Aqui a tabela de clientes seria a principal tabela Fato, enquanto todas as outras seriam tabelas adjacentes que caracterizam, ou dão informações, á tabela de clientes. 
## **FUNÇÕES DAX**

### O que são:

As funções DAX são como funções e operações no Excel. São elas que permitem o calculo efetivo dos valores que serão aplicados no Relatório. As funções DAX podem ser utilizadas tanto para medidas quanto para colunas calculadas.

### Sintaxe e operadores

Para iniciar uma formula DAX: selecione uma coluna> clique com o botão direito> nova coluna / Nova medida

A sintaxe das funções DAX seguem este padrão: "nome da coluna" = "Funções e operações".

Os operadores principais são:
Adição: +
Subtração: -
multiplicação:  *
Divisão: /
potenciação: ^

OBS: Utilizar o TAB para selecionar as colunas, pois o ENTER serve para finalizar a formula

Operadores de comparação:

os operadores de comparação no Power BI são:
Maior que: >
Menor que: <
igual á: =
Maior ou igual: >=
Menor ou igual: <=
Diferente de: <>

Operadores Especiais:

Os operadores especiais no Power BI são:

Concatenar: &
E: &&
OU: ||

IN: Este operador é usado quando se tem mais de uma verificação condicional "OU" para uma mesma coluna, em outras palavras, ele vai verificar um Escopo de opções onde ao menos uma delas pode ser verdadeira

![[Pasted image 20241116210740.png]]

neste exemplo, é verificado se os valores de nível importância aderem a um dos critérios estabelecidos dentro do IN, ou seja, se há os valores 1, 2 ou 3. Se ao menos um dos valores existir o resultado será verdadeiro.

A sintaxe dele é: IN{Critério de avaliação}.

*Uma aplicação dentro de IF*
![[Pasted image 20241116211200.png]]


### Formulas

#### Formulas SE

A formula "SE" verifica se uma condição é verdadeira ou falsa, nela podem ser usados os operadores de comparação como AND(&&), ou OR(||). elas são escritas em inglês igual nas linguagens de programação, portanto: IF(Condição; valor se verdadeiro; Valor se falso). 

Caso sejam usados os operadores de comparação por extenso, ela ficaria da seguinte forma: IF(AND/OR()), sendo necessário passar primeiro a comparação dos operadores e depois os resultados do IF. 

Caso sejam usados os operadores com os símbolos, ela ficaria da seguinte forma:
IF(condição &&/|| Outra condição; resultado se verdadeiro; resultado se falso).

*Exemplo de IF Escrito por Extenso:* ![[Pasted image 20241124195557.png]]
*Exemplo de IF Escrito com Símbolos:* ![[Pasted image 20241124195501.png]]

As formulas "SE" ainda podem estar Aninhadas, ou seja, uma "SE" dentro da outra, caso seja feito desta forma ela ficará assim: 
IF(Condição; Resultado se verdadeiro; IF(Condição; Resultado se verdadeiro; Resultado se falso))
Neste caso, podemos ter vários IF no resultado se falso, sendo assim o IF aninhado serve como um ElseIF.

*Exemplo de IF aninhado:* ![[Pasted image 20241124200844.png]]

OBS: É possível quebrar linhas nas formulas clicando com Shift+Enter: ![[Pasted image 20241124201032.png]]


#### Formulas de Texto
São formulas DAX para a manipulação de texto, apesar de não serem tão utilizadas algumas interessantes são:

LEFT, RIGHT, MID: Destacam uma parte do texto na direção indicada pela formula, ou seja, a esquerda, direita ou no meio, é escrita desta forma: 

LEFT/RIGHT(coluna a ser manipulada, quantos caracteres quer destacar);
MID(Coluna a ser manipulada, ponto de inicio, quantos caracteres quer destacar)
OBS: Pode ser colocado na MID um numero grande, pois, ele vai pegar os caracteres até o final sem deixar maiores espaços, então se a coluna possuir três caracteres do ponto inicial ao final ele pegará somente estes três, ele não criara mais caracteres vazios até a quantidade do numero grande.

Assim, se for usada a LEFT, ele destacará os primeiros caracteres a esquerda, se for usada a RIGHT, será os dois primeiros caracteres a direita, se for o MID, serão os dois caracteres do centro.

*Exemplo LEFT:*
![[Pasted image 20241124234051.png]]

*Exemplo RIGHT:*
![[Pasted image 20241124234121.png]]

*Exemplo MID:*
![[Pasted image 20241124234154.png]]


TRIM: A formula TRIM retirara quaisquer espaços extras no texto, é escrita desta forma: TRIM(Coluna a ser manipulada). Ela não retira os espaços originais da coluna, ou seja, os espaços específicos dela para separação própria.

SERACH: Procura um caractere especifico e retorna sua posição, é escrita desta forma:
SEARCH(Texto procurado; coluna para ser vasculhada; posição inicial; valor se o texto não for encontrado). Nesta função os dois últimos parâmetros são opcionais.

*Exemplo de SEARCH:*
![[Pasted image 20241124235613.png]]

#### Formulas de data

São fórmulas para manipulação de datas, as mais comuns são a DAY, MONTH, e YEAR, para extrair o dia mês e ano. Elas são escritas desta forma:

DAY/MONTH/YEAR(Coluna com a data)

*Exemplos:*
![[Pasted image 20241125001501.png]]

![[Pasted image 20241125001520.png]]

![[Pasted image 20241125001538.png]]


É importante que os dados estejam formatados como data.

Mas não é necessário utilizar estas formulas para pegar estas informações, caso a coluna esteja com formato de data é possível pegar os dados passando um parâmetro na coluna, se escreve desta forma: coluna a ser pesquisada.[Ano/Mês/Dia].

*Exemplos:*
![[Pasted image 20241125001840.png]]

![[Pasted image 20241125001858.png]]

![[Pasted image 20241125001919.png]]

End Of Month: Retorna o ultimo dia de um mês, se escreve desta forma:

EOMONTH(Coluna a ser vasculhada; intervalo de tempo em relação a coluna).

O segundo parâmetro pede um intervalo de tempo, ou seja, se será verificado o mês da coluna, algum mês antes ou algum mês posterior. Para verificar estes dados basta colocar um numero negativo(para meses anteriores), o numero zero(para o mês atual), um numero positivo(Para meses posteriores). 

Exemplos:
*Retorna o ultimo dia do mês atual*
![[Pasted image 20241125003152.png]]

*Retorna o ultimo dia daqui a dois meses*
![[Pasted image 20241125003240.png]]

*Retorna o ultimo dia de dois meses atrás*
![[Pasted image 20241125003338.png]]

DATEDIFF(Diferença de datas): Esta formula retorna a diferença entre duas datas especificadas usando algum tipo de intervalo, como dias, meses, anos, trimestres, etc.
É usado com a função TODAY, que retorna a data atual, e é uma opção melhor para o calculo de idades. É escrita desta forma:

DATEDIFF(data inicial, data final, intervalo em dias, meses, anos, etc.)
TODAY(). (Sim, sem nenhum parâmetro)

*Exemplo:*
![[Pasted image 20241125003639.png]]
##### Função Related:

A função Related importa os dados de outras tabelas, ela se escreve desta forma:

RELATED(Nome da tabela[Coluna da tabela])

*Exemplo:*
![[Pasted image 20241125005158.png]]

### Medidas

Medidas são formulas DAX utilizadas para resumir colunas ou tabelas, ou seja, para somar todas as linhas de uma coluna, contar os itens delas, verificar algo especifico na tabela, etc.

Elas são criadas da mesma forma que uma coluna calculada, porem é selecionada a opção nova medida ao invés de nova coluna.

OBS: Nas medidas as colunas não podem ser usadas sem uma formula, a menos que o dado utilizado já seja uma medida.

OBS2: As principais diferenças entre uma medida e uma coluna calculada é que, a primeira faz apenas um calculo e o deixa armazenado na memoria, enquanto a ultima cria efetivamente uma nova coluna na tabela com os valores da função. E, a primeira exige uma formula para ser utilizada, enquanto a ultima não tem tal exigência.
#### Operações Básicas

As operações básicas são: SUM, AVERAGE, MAX, MIN, e são escritas desta forma:

SUM(Coluna a ser somada).

OBS: Uma nota é que elas não criam uma nova coluna, como nas colunas calculadas, elas criam apenas uma medida que deve ser utilizada no relatório, e é nele que você verificara se a formula esta funcionando corretamente.

#### Operações de contagem

As operações de contagem são: COUNT, COUNTA, COUNTROWS, e DISTINCTCOUNT, elas todas são diferentes entre si, mas são escritas da forma: 
COUNT(Coluna a ser contada)

COUNT: Esta formula conta apenas os números em uma coluna, ou seja, caso hajam textos nesta coluna esta formula não funcionara.

COUNTA: Esta formula conta todos os valores em uma coluna, independente de seu tipo.

COUNTROWS: Conta as linhas preenchidas em uma coluna ou tabela.

DISTINCTCOUNT: Conta apenas os valores distintos em uma coluna, ou seja, só conta os valores uma vez, não os repetindo.

#### CALCULATE

A formula CALCULATE executa uma operação dado algum tipo de filtro, portanto, a operação será executada somente quando o filtro for verdadeiro. É escrita desta forma:
CALCULATE(operação; Filtros a serem utilizados).

Notas: 

Os filtros utilizados devem ser como uma comparação, ou seja, se um valor é igual, maior, menor, menor ou igual a outro, etc. 

É importante que a coluna utilizada para filtros não seja usada como um filtro no relatório, pois o filtro do calculate possui prioridade em relação aos outros filtros, então ele vai sobrepor todos os outros. 

Por fim, não é possível utilizar qualquer formula ou medida nos filtros do calculate puro, somente aquelas já disponibilizadas para o segundo parâmetro em diante.

ALL: Um dos filtros que podem ser utilizados como segundo parâmetro é o ALL, este filtro indica que aquela operação deve ser feita para todos os valores independente dos filtros ou índices. Então sim, ele é um filtro que faz a função ignorar qualquer outro filtro para aplicação. Ele é escrito desta forma: 
ALL(Tabela ou coluna a ser aplicado).

Junto com a calculate:
CALCULATE(operação a ser realizada; ALL(Coluna ou tabela a ser aplicado))

![[Pasted image 20241201011356.png]]

FILTER: Esta formula pode ser utilizada como segundo parâmetro da calculate, e permite a utilização de medidas como filtro do calculo, ele acaba não sendo muito utilizado por tornar o relatório mais pesado e por ser um pouco mais complexo de escrever, mas ele é escrito desta forma: FILTER(tabela a ser aplicado o filtro; filtro a ser aplicado)

junto com Calculate:
CALCULATE(Operação a ser realizada; FILTER(Tabela a ser aplicado o filtro; Filtro a ser aplicado))

![[Pasted image 20241201011648.png]]
#### Funções iterativas

Realiza uma operação em todas as linhas de algumas colunas em uma tabela, criando uma coluna imaginaria com os resultados dessa operação e, no final, realizara uma outra operação em cima dos valores finais calculados. As principais formulas são, SUMX, AVARAGEX, MAXX, MINX, COUNTX.
São escritas desta forma: SUMX(Tabela onde será feita a expressão, expressão a ser feita primeiro)

OBS: Na parte da expressão podem ser utilizadas outras formulas diversas.

OBS2: Esse tipo de medida pode ser utilizado caso não seja necessária a criação de alguma coluna intermediaria para algum calculo, podendo assim fazer a operação de maneira mais direta.

Por Exemplo: SUMX(Base Clientes, VT + VR + Benefícios). A função somara as linhas de cada coluna separadamente, depois criará uma coluna imaginaria com os resultados da soma, por fim fara a soma de todos os valores desta coluna imaginaria, este será o resultado final da medida

![[Pasted image 20241130231712.png]]

AVARAGEX: Retorna o valor médio de uma tabela após uma dada operação.

![[Pasted image 20241130232813.png]]

MAXX: Retorna o valor máximo em uma tabela após uma dada operação, o MINX retornara o menor valor.

![[Pasted image 20241130233153.png]]

![[Pasted image 20241130233320.png]]

COUNTX: Retorna a quantidade de números em uma tabela após uma dada expressão

## **RELATORIOS**

Os relatórios são a parte visual do Power Bi, é o finalmente após todo o tratamento dos dados, é nele que serão montados os dashboards para analisar as informações e dados de maneira visual e intuitiva. Neles temos varias ferramentas, desde matrizes a gráficos e mapas, eles serão explicados aqui.

### Elementos:
Dentro do Power Bi é possível escolher elementos para estilizar os relatórios, eles vão além das ferramentas de analise pois servem mais para contextualizar ou estilizar os relatórios, eles ficam na guia inserir e podem ser estilizados nas caixas ao lado:

![[Pasted image 20241207145421.png]]

![[Pasted image 20241207145538.png]]
### Gráficos de coluna e barras

Os gráficos de colunas e barras se dividem em dois tipos, os empilhados e os clausterizados, no fundo ambos fazem a mesma coisa, porem de formas diferentes. os gráficos de coluna empilhados ficam um sobre o outro, enquanto os clausterizados ficam um ao lado do outro, portanto a principal diferença é estética. Ambos os gráficos possuem os campos de eixo, legenda, e dicas de ferramentas. nos Eixos ficarão os índices e valores do gráfico, nas legendas ficarão algumas informações adicionais do gráfico (como uma legenda dele mesmo), e no campo de dicas de ferramentas ficarão informações adicionais que não precisam ser mostradas explicitamente, sendo assim essas informações aparecerão somente quando o mouse for passado por cima delas.

![[Pasted image 20241207150552.png]]Á esquerda o gráfico de barras empilhado e a direita o de colunas clausterizado

![[Pasted image 20241207150707.png]] ![[Pasted image 20241207150835.png]]
Campos de ambos os gráficos e exemplo das dicas de ferramentas

### Gráficos de linhas e de áreas

A separação dos gráficos de área e linha são estéticas, pois ambos servem para a mesma finalidade, verificar uma informação em um período. A escolha de um ou outro pode depender do tipo de dado analisado e do volume deles, pois com muitos dados um pode ficar mais confuso do que o outro. 

O gráfico de linha traça uma ou varias linhas dado um período e certos valores, mas ele não sombreia uma área abaixo dele, já o gráfico de área faz um sombreamento além das linhas.
Os campos para eles são, eixo X, eixo Y, eixo Y secundário, as legendas, e as dicas de ferramentas.
O mais diferencial neles é o eixo Y secundário, ele permite criar um segundo parâmetro de índices, permitindo uma comparação semelhante a um gráfico de área ou linha empilhado, o resto dos campos permanecem iguais.

Gráfico de área simples:
![[Pasted image 20241207161433.png]]

Gráfico de área com eixo Y secundário
![[Pasted image 20241207161555.png]]

Gráfico de linhas
![[Pasted image 20241207161853.png]]

Gráfico de área empilhado
![[Pasted image 20241207162805.png]]

Obs.: Quando se possui datas ou informações com uma certa Hierarquia no gráfico, é possível transitar entre os níveis de hierarquia ao clicar nas setas presentes no campo superior esquerdo. As datas por exemplo possuem a Hierarquia: Ano> Trimestre> mês> Dia, ao se clicar nas setas é possível transitar entre essas hierarquias filtrando os dados por alguma delas.

### Gráficos compostos
Os gráficos compostos juntam os gráficos de linhas e colunas em um só, permitindo a contagem de duas ou mais informações em um gráfico compartilhado. Os principais campos são o Eixo X, Eixo Y da Coluna, Eixo Y da linha, e Legenda da coluna, os outros campos ficam iguais.

O Eixo X são os valores compartilhados tanto pela linha quanto pela coluna, por isso pode ser bom utiliza-los como um índice.

O Eixo Y da coluna define os valores que serão utilizados nas colunas em Si, enquanto o Eixo Y da linha definem os valores a serem utilizados nas linhas.

A legenda da Coluna são as legendas do gráfico, são utilizadas somente nas colunas pois elas fazem a maior parte da separação das informações.

As dicas de ferramentas também são compartilhadas tanto pela linha quanto pelas colunas.

Gráfico de coluna e linha empilhada
![[Pasted image 20241207164831.png]]

### Filtros

Há duas formas de Filtrar as informações no Power BI, selecionando alguma informação no relatório(Como alguma coluna em um gráfico ou uma linha em uma tabela), ou utilizando o campo de filtros diretamente. Se for utilizado o filtro selecionando alguma informação no relatório, este será aplicado para todos os elementos naquela pagina do relatório, não apenas para o gráfico ou coluna selecionada.

![[Pasted image 20241208190420.png]]

Se for utilizado o campo de filtros serão dadas três informações principais, o filtro neste Visual(No elemento selecionado), o Filtro nesta pagina, ou o filtro neste relatório todo. 

#### Configurações do Filtro

O filtro neste visual aplica o filtro somente no elemento selecionado, não influenciando os outros elementos do relatório.

Filtro Aplicado somente no primeiro gráfico
![[Pasted image 20241208190851.png]]

Além dessa filtragem básica, é ainda possível selecionar dois tipos diferentes de filtragem, a filtragem avançada e a N Superior. 

A filtragem Avançada permite o uso de comparações de valores, ou seja, se será filtrado quando conter um valor, quando o valor for menor ou maior que outro, etc. Neste tipo de filtragem é possível selecionar mais de uma comparação, utilizando o "E" ou "OU".

Filtragem Avançada
![[Pasted image 20241208191522.png]]


A filtragem N superior seleciona os N maiores ou menores valores baseados em um critério, por exemplo, seleciona os três maiores valores se baseando no total de vendas, sendo assim será selecionado as três maiores vendas, a mesma logica serve para os menores valores. O critério será uma coluna a ser escolhida.

Filtro N superior
![[Pasted image 20241208192050.png]]

Os filtros "nesta Pagina" e "Neste relatório" possuem as mesmas configurações, porem o primeiro aplica o filtro para todos os elementos naquela pagina(Como se fosse uma seleção direta) e o segundo aplica o filtro para todas as paginas do relatório.
OBS: Os filtros dependem bastante das relações entre as tabelas, sendo assim deve-se atentar bastante neste ponto.
OBS²: Quando um filtro não puder ser aplicado o Power Bi recusará sua inserção.

Filtro "Nesta Pagina"
![[Pasted image 20241208193322.png]]

Filtro "Neste relatório"
![[Pasted image 20241208193448.png]] ![[Pasted image 20241208193508.png]] ![[Pasted image 20241208193541.png]]

#### Formatação condicional

A formatação condicional esta disponível para as tabelas e matrizes, ela permite realçar as linhas a partir de uma condição já pronta ou uma condição criada pelo usuário, para criar uma condição basta clicar no botão de formula.

![[Pasted image 20241208195622.png]] ![[Pasted image 20241208195647.png]]

OBS: Em algumas versões o nome esta como "Elementos da célula" e dependendo da formatação ou da coluna escolhida a segunda tela pode mudar.

#### Segmentação de Dados

A segmentação de dados é um elemento do relatório que cria um botão flutuante de filtros.

![[Pasted image 20241208201632.png]]

A segmentação aparece de forma diferente quando se trabalha com datas, ela permite a seleção por datas especificas, por meses, por ano, entre outros. uma das formas de data que ela permite colocar são as datas relativas, ou seja, a seleção dos dados em um certo período de tempo , e não em uma data especifica.

Formato de Data Relativa
![[Pasted image 20241208203632.png]] 

Formato Padrão de segmentação de data
![[Pasted image 20241208203702.png]]

Para aplicar a segmentação de dados de uma pagina para as outras de um relatório, basta: selecionar a guia "Exibição"> "Segmentação de dados de Sincronização"

![[Pasted image 20241208204126.png]]

nesta tela você poderá selecionar as paginas onde a sincronização será aplicada e em quais delas a caixa de segmentação aparecerá

![[Pasted image 20241208204233.png]]

### Cartões

Os cartões são elementos no Power BI que servem para destacar uma ou mais informações, sejam elas números ou textos, para isso eles se dividem em dois tipos, o cartão simples e o cartão múltiplo. Essencialmente eles fazem a mesma coisa, porem o cartão simples mostra apenas uma informação enquanto o cartão múltiplo pode mostrar mais de uma.

*Elementos de cartão*
![[Pasted image 20241214114054.png]]

*Exemplo de cartão múltiplo à esquerda e cartão simples à direita*
![[Pasted image 20241214114317.png]]

É possível colocar colunas de texto nos cartões, fazendo assim uma indicação mais direta de algo, e para estes casos é recomendado o uso dos filtros para especificar as informações.

*Cartão de texto com filtro*
![[Pasted image 20241214120209.png]]

### Gráfico de Pizza e anel

Os gráficos de Pizza e anel servem ao mesmo proposito, representar por meio de fatias uma certa porcentagem, a diferença entre eles é principalmente estética. O principal campo que o distingue dos outros gráficos é o "Detalhe", enquanto a legenda divide o gráfico em grandes setores, o detalhe divide o gráfico em setores menores.

![[Pasted image 20241214123839.png]]

![[Pasted image 20241214121725.png]]

#### TreeMap

O treeMap é o mais diferente dos gráficos, isso porque ele faz a separação dos valores em caixas, estas aumentam ou diminuem a depender do valor, os campos são iguais aos mapas de pizza e anel, somente mudando o nome de "legenda" para "Categoria". Ele é particularmente útil quando se tem diversos valores.

![[Pasted image 20241214123016.png]]

### Mapas

Os mapas são elementos no Power BI que permitem a quantificação de algo em alguma posição geográfica, essa quantificação será representada no mapa. Existem três tipos principais de Mapas, o normal, o coroplético, e o ArcGis. Eles possuem algumas configurações diferentes um do outro, mas os principais entre eles são os campos de localização, latitude e longitude. A localização busca por um endereço ou local especifico, a latitude e longitude servem ao mesmo proposito, mas podem ser usados caso não se possua uma localização.

Para se utilizar os gráficos são necessárias duas coisas principais, uma base de endereços, para servir de referencia, e uma conexão com a internet, para que o Power Bi possa fazer as consultas de localizações. Além disso é importante se atendar nos relacionamentos entre a base de endereços e as outras bases, pois a partir do relacionamento que as informações serão divididas.

Dentro do mapa, os campos para endereço devem ser colocados em localização(ou em Lat. Long. se estiver os usando), e as informações a serem mostradas irão em "Dicas de ferramentas" ou em "Legendas".


A principal diferença entre o mapa comum e o coroplético é que o primeiro representa as quantidades por bolhas no mapa, estas aumentam ou diminuem dependendo dos valores, e o ultimo pinta no mapa todos os locais de sua base, e indica os valores ao passar o mouse por cima das áreas, este acaba sendo mais propicio a formatação condicional com gradiente de cores.

*Exemplo de mapa comum à esquerda e mapa coroplético à direita*
![[Pasted image 20241214165151.png]]



### KPI's e Fórmulas de tempo

São indicadores que retornam alguma média ou valores em um dado período de tempo, no mais servem para fazer indicações em certos períodos, mostrando aspectos como metas e valores reais.

#### Fórmulas de inteligência de tempo

As formulas de inteligência de tempo servem para medir vários períodos diferentes, e para isso é necessário uma base calendário que contenha todas as datas que serão utilizadas, e esta base deve ser diária, ou seja, progredir dia após dia dada uma data inicial.

Como a ideia é comparar períodos em anos diferentes, é necessário que o período em ambos os anos estejam em uma mesma coluna, para isso é recomendado o uso da função "StartOfMonth", pois ela retornará o dia de inicio de cada mês ao longo da coluna, permitindo assim a comparação de certos meses em anos diferentes.   
##### Construção da Base calendário

há duas formas de construir uma base calendário, ambas utilizando funções DAX. A primeira é utilizando a função "Calendar", esta criara um calendário a partir uma data inicial e final. A outra é usando a função "CalendarAuto", esta criará um calendário a partir das datas iniciais e finais de toda a sua base de dados, porem, esta ultima não aparece no editor de consultas e mais pesada para execução do que a função "Calendar".

![[Pasted image 20241215205418.png]]
![[Pasted image 20241215205818.png]]

Independente de qual função for utilizada, é possível extrair os elementos menores da data (Como Ano, mês e dia).

##### Parâmetro DATEADD

O parâmetro DateAdd é um dos filtros da função "Calculate", ela retorna os valores de uma certa data anterior, para isso ela requisita a matriz de data a ser analisada, o período a ser analisado(ou seja quantos X valores a frente ou atras), e o tipo do período a ser analisado(ou seja, se a analise será feita por ano, dia, mês, etc.)

![[Pasted image 20241215212154.png]]

##### Parâmetro DATESYTD

O parâmetro DATESYTD é um dos filtros do "Calculate", ele faz um calculo apenas dentro dos anos de sua base, ou seja, se você possuir em sua base os anos 2000, 2001, e 2002, ele fará um calculo separado para cada ano, sem efetuar o calculo com os valores do ano anterior ou seguinte. Seu principal requisito são as datas para serem usadas de parâmetro

![[Pasted image 20241215221158.png]]
#### Elemento KPI

O KPI é um elemento que retorna o desvio de um valor em relação a muta em um dado período, seus principais campos são, os valores a serem analisados, o período a ser analisado(Neste caso ele retorna por padrão a ultima data), a meta a ser comparada. 

![[Pasted image 20241215214513.png]]

## **OUTROS**

### Tabela de medidas

Para organizar melhor os dados, é possível criar uma tabela somente para as medidas, isso é feito da seguinte forma:

primeiro é necessário criar uma nova tabela, para isso deve-se clicar em "inserir dados" > carregar

![[Pasted image 20241222164501.png]]

Após isso há duas formas de se colocar as medidas na tabela. 

Para a primeira delas selecione a guia "Relatório" > selecione uma medida> clique em "tabela inicial" na guia de ferramentas de medida> selecione a nova tabela criada.

![[Pasted image 20241222164744.png]]

Para a segunda delas, selecione a guia de "Relacionamentos"> encontre as medidas nos campos laterais> e arraste-as para a nova tabela criada.

![[Pasted image 20241222165010.png]]

Após colocar as medidas nesta nova tabela, oculte a coluna que foi criada, com isso o Power Bi entenderá aquela tabela como uma própria para medidas e a colocará no topo da guia dados.

É ainda possível criar pastas dentro da tabela de medidas para organiza-las ainda mais. Para isso: vá na guia de "Relacionamento"> selecione uma medida> no campo de "Propriedades" encontre o campo "Pasta de exibição"> de um nome para a pasta. Isso vai criar uma pasta onde é possivel guardar medidas dentro delas.

![[Pasted image 20241222165920.png]]

### Gráfico de Funil

O gráfico de funil serve para segmentar os valores inseridos em diversas etapas, por mais que sua utilidade seja muito similar a um gráfico de linha comum, o de funil se destaca por inerentemente permitir a comparação dos valores atuais com os anteriores. 

Para sua construção, o gráfico de Funil pede dois parâmetros principais: A categoria e os valores, com o primeiro sendo a forma como os valores serão segmentados, ou divididos.

![[Pasted image 20241222210239.png]]


No gráfico de filtro temos duas informações interessantes, ele naturalmente permite a comparação com o campo anterior e com o primeiro campo, mostrando a diferença entre eles, esta aparece em porcentagem, mas pode ser formatada conforme a necessidade. Os números no topo e no fundo representam a porcentagem em relação ao primeiro valor, dessa forma, o primeiro campo representa 100% do primeiro valor enquanto o ultimo campo representa 19,4% do primeiro valor.

![[Pasted image 20241222210955.png]]

### Hyperlinks

Os Hyperlinks são botões dentro do relatório que direcionam o usuário para outras partes do mesmo, assim não seria necessário ficar clicando nas páginas para ir á outra parte do relatório, basta clicar em um botão com um link e você será redirecionado para lá.

Para criar os Hyperlinks é necessário seguro alguns passos:

1º Selecionar um botão: para isso vá na guia "Inserir" e selecione uma forma ou um botão, e diminua sua transparência para a mínima caso esteja usando algum ícone importado.

![[Pasted image 20241222212825.png]]

![[Pasted image 20241222213036.png]]


2ª Indicar uma ação: para indicar ao Power Bi para ir a alguma pagina precisamos: Selecionar a forma> habilitar o campo "Ação"> definir o tipo de ação como "indicador"> selecionar para onde aquele botão vai indicar.

De inicio, as paginas não aparecerão, pois elas por padrão não aparecem como uma pagina para ser indicada, para mudar isso: Selecione a página do relatório desejada> Clique na guia "Exibição"> clique na opção "Indicadores"> clique em "Adicionar". Isso fará com que esta pagina selecionada possa ser indicada em um hyperlink.  

*Campo de indicadores no botão*
![[Pasted image 20241222213945.png]]

*Campo que define uma página para ser indicada*
![[Pasted image 20241222214035.png]]

Dentro do Power Bi um link será seguido ao clicar no botão segurando CTRL. Mas quando o relatório for publicado o link será seguido assim que clicado.

### Visuais como dicas de ferramentas(Tooltip)

É possível configurar uma pagina do relatório com vários visuais para ser uma dica de ferramenta(ou tooltip), sendo assim é possível colocar gráficos dentro de gráficos, ou cartões dentro de cartões, a seguir o passo a passo de como fazer isso.

primeiro, é necessário habilitar uma pagina para ser uma dica de ferramenta e configura-la. Para habilitar uma pagina a ser usada como tooltip, crie uma nova pagina de relatório e vá em formato da pagina> informações da pagina> e selecionar a opção para permitir usar esta como uma dica de ferramenta.

![[Pasted image 20241225123632.png]]

neste ponto a tela deve ser redimensionada automaticamente para a resolução de uma tooltip mas, caso isso não tenha ocorrido, na mesma guia clique em "Configurações de tela"> Tipo> Dica de ferramenta

![[Pasted image 20241225123842.png]]

Com isso a pagina já esta configurada para ser utilizada como uma dica de ferramenta. O próximo passo é montar os gráficos ou indicadores que deseja e colocar esta pagina, efetivamente, como uma dica de ferramenta em outro gráfico.

Para colocar a pagina criada como Tolltip em outro gráfico, selecione o gráfico desejado> clique para formatar o visual dele> clique na guia geral> clique em dicas de ferramentas> no tipo selecione "Pagina de relatório"> em pagina selecione a pagina criada e definida como tooltip.

Com isso a tooltip já estará habilitada naquele gráfico:

![[Pasted image 20241225125731.png]] ![[Pasted image 20241225125753.png]]


### Tabela calendário(Power Query)

Código para criar Base de Calendário e Datas (Dentro do Power Query!!):

= List.Dates(#date(1900,1,1), Number.From(DateTime.LocalNow())-Number.From(#date(1900,1,1)) ,#duration(1,0,0,0))

### Como criar Rankings

