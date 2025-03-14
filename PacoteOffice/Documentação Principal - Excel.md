#pacoteOffice 
## Conceitos Básicos

### Abas do Excel

O Excel é dividido em oito abas principais, cada uma gerenciando um conjunto de ferramentas do Excel. São nessas abas que serão selecionados os elementos que compõem o relatório.
#### Pagina inicial

Na pagina inicial temos algumas ferramentas gerais para a manipulação dos dados no Excel, como a formatação da fonte e alinhamento dos dados, os tipos de dados, a estilização de células ou tabelas e a inserção ou remoção de linhas e colunas.

![[Pasted image 20241207233704.png]]

##### Formatações de texto

As formatações de texto podem ser feitas na página inicial do Excel, utilizando os campos "Fonte" e "Alinhamento". No primeiro campo é possível modificar o tipo de fonte utilizado no texto de uma célula ou em um conjunto de células, o tamanho desta fonte, se o texto será negrito, sublinhado ou rasurado, a quantidade de bordas que as células terão,( ou seja, se terão bordas em todos os cantos ou apenas em um lado especifico), e por fim é possível preencher a célula com alguma cor ou mudar a cor da fonte a fonte.

No segundo campo, é possível modificar os alinhamentos vertical e horizontal do texto,  mudar sua orientação(ou seja, se o texto ficará na horizontal, vertical, ou na diagonal, aqui é possível mexer no grau do texto para sua orientação), modificar seu recuo á direita ou esquerda, habilitar a quebra automática de texto e, por fim, é possível mesclar e centralizar as células, isso faz com que varias células sejam somente uma e centraliza o texto da célula superior esquerda.

![[Pasted image 20241231182009.png]]

#### Adição e exclusão de linhas e colunas

A adição de linhas pode ser feito no campo células, ou clicando com o botão esquerdo em um índice de linha> inserir, a adição é feita abaixo da linha selecionada e mantem a formatação da linha acima. A exclusão remove a linha selecionada e pode ser feita da mesma forma. O mesmo serve para as colunas, com exceção de que estas só podem ser adicionadas ou excluídas com o botão esquerdo do mouse. É ainda possível adicionar ou remover planilhas inteiras nos mesmos campos, e a formatação de tamanho e exibição de linhas e colunas pode ser feita no mesmo campo, na opção "Formatar".

![[Pasted image 20241231184538.png]]

#### pagina Inserir

Na guia inserir temos algumas ferramentas mais avançadas do Excel, como as tabelas dinâmicas, informações suplementares, gráficos, filtros e links.

![[Pasted image 20241207233730.png]]

#### Pagina Desenhar

Nessa pagina é possível fazer desenhos e marcações á mão no relatório
![[Pasted image 20241207233827.png]]

#### Pagina Layout

Nessa pagina é possível gerenciar as configurações de impressão e exibição do formulário, ela contem temas, configurações de margem e tamanho de pagina, exibição ou não das linhas de grade e títulos e outras ferramentas de visualização de dados

![[Pasted image 20241207234038.png]]

#### Pagina de Formulas

Nessa pagina há uma biblioteca com as principais formulas do Excel dividas por categorias, além das ferramentas de gerenciamento de nomes e validação das formulas

![[Pasted image 20241207234222.png]]

#### Pagina de Dados

Nessa pagina podem ser gerenciados os dados que alimentam o Excel, permitindo selecionar de onde eles vem, filtrar ou classificar os dados e aplicar outras ferramentas de validação e gerenciamento, como a remoção de duplicatas e erros, e a transformação dos dados para colunas.

![[Pasted image 20241207234430.png]]

#### Pagina de revisão

A pagina de revisão permite adicionar elementos de orientação e segurança a tabela, com os comentários, revisões de texto e proteção de planilhas ou arquivos 

![[Pasted image 20241207234608.png]]

#### Pagina Exibir

Nessa pagina é possível gerenciar a estilização da planilha, mudando o modo de exibição, selecionando se as linhas de grade ou outros elementos aparecerão na planilha, fazendo o gerenciamento de janelas, e por fim permitindo a criação de Macros

![[Pasted image 20241207234858.png]]

### Tipos de Dados

Ao fazer a inserção de algum dado no Excel ele não fará a identificação automática do tipo de dado, ele marcará o dado como 'Geral'. A alteração do tipo de dado pode ser feito na pagina inicial, no campo de números. Nessa tela é possível mudar o tipo de dado e sua formatação, por exemplo, se for um numero com casas decimais é possível alterar a quantidade de casas decimais nele, é possível fazer a separação por milhares, se for um texto é possível mudar todos os elementos da fonte, Etc. 

![[Pasted image 20241207235723.png]]

Demais opções de formatação e outros tipos de valores podem ser encontrados na opção "Mais formatos de números", ou "Formatar Células"(A setinha com a diagonal inferior direita)

Aqui é possível modificar o tipo de dado e selecionar uma formatação especifica para ele, além de ser possível modificar os estilos das células, ou seja, suas boras, cores, estilos da fonte, alinhamento, etc.

![[Pasted image 20241207235925.png]]


Algumas observações a serem feitas são: Números são por padrão colocados à direita da célula, textos à esquerda da célula. O tipo de dado moeda deve ser alterado na guia pagina inicial, se a moeda for colocada antes do número ele só reconhecerá aquela de seu país, se outra moeda for colocada ele reconhecerá o valor na célula como um texto. O tipo de dado selecionado fica gravado na célula mesmo após a exclusão de seu valor. 

Sobre a porcentagem, caso a célula não possua valor o Excel entende que 1 = 100%, portanto, caso deseje um valor menor, ele deve ser colocado como 0,x, que representa uma fração destes 100, mas caso a célula já esteja formatada como porcentagem antes de haver um valor, o Excel reconhecerá as unidades normalmente. Para Exemplificar, caso haja o valor 9 em uma célula e esta seja depois formatada como porcentagem, o Excel reconhecerá o 9 como 900%, mas caso a célula seja formatada antes da inserção do número, o Excel reconhecerá o 9 como 9%.


### Planilhas

As planilhas, ou pastas de trabalho, são os principais ambientes do Excel, é nelas que estão contidas as células e todas as paginas para o gerenciamento e tratamento dos dados. O principal gerenciamento das planilhas pode ser acessado ao se clicar com o botão direito em cima de uma delas, assim são liberadas opções como inserir planilhas especificas, renomear ou excluir a planilha, move-la para alguma outra posição, ou alterar sua cor para organização.

![[Pasted image 20241231174134.png]]

#### Formatação Estrutural

Alguns outros pontos são: O nome de uma planilha não pode ficar em branco e não pode conter alguns caracteres, como, " \ ", " / ", "?", entre outros.

A navegação nas planilhas pode ser feita utilizando as teclas: TAB(Para deslocar para célula á direita), SHIFT(Para deslocar para as células abaixo), ou as setas do teclado(para se mover para qualquer direção).

O tamanho de uma célula pode ser modificado ao arrastar o índice da coluna para os lados, ou ao clicar duas vezes entre um índice e outro com algum conteúdo na primeira linha da célula, o mesmo se aplica para as linhas.

É possível modificar mais de uma célula ao selecionar duas ou mais ao mesmo tempo, isso pode ser feito clicando e arrastando o mouse nas células. 

### Fórmulas Básicas

Antes das formulas propriamente ditas falemos dos operadores:

"+" é para adição
"-" é para Subtração
" * " é para Multiplicação
" / " é para Divisão
" ** " é para Potenciação

Diferente do Power BI, não é possível utilizar && ou || para as condições lógicas, sendo necessário utilizar as formulas "E" e "OU"

As formulas básicas podem ser divididas em alguns grupos, como formulas matemáticas, formulas de contagem e formulas condicionais.

As formulas matemáticas básicas são: SOMA, MULT, MÁXIMO, MÍNIMO, MÉDIA; Que executam as respectivas operações em duas ou mais células.

As fórmulas de contagem são: CONT.NÚM, CONT.VALORES, CONTAR.VAZIO; elas contam, respectivamente, células que possuem apenas números, células que possuem qualquer valor, e células que não possuem nenhum valor.

As fórmulas condicionais são, num geral: SE(S), E, OU, CONT.SE(S), SOMA.SE(S), SEERRO. Elas serão tratadas mais afundo na parte de de condições, mas num geral, elas verificam se uma condição é verdadeira, se for verdadeira executam uma ação, se for falsa executam outra. As formulas E/OU servem para adicionar mais de uma condição, a primeira será verdadeira quando todas as condições forem verdadeiras, e a segunda será verdadeira se ao menos uma for verdadeira.

#### Referencias de células

É possível criar formulas referenciando células na mesma aba ou em abas diferentes, para isso basta selecionar as células desejadas, mas, se quiser referenciar outra aba é necessário colocar o nome dela antes da célula desejada. Além disso é possível copiar e colar as formulas para as outras células, o Excel manterá o intervalo e o acompanhará, a menos que as células sejam trancadas, movidas, ou recortadas e coladas em outro lugar.

Esse acompanhamento é chamado de referencia relativa, pois os valores são relativos á célula, ou seja se o ultimo muda o primeiro muda também. Em contraponto temos a referencia Absoluta , ou trancamento, que diz para o Excel que certas células sempre serão referencia, não importando se a fórmula mudar de lugar, isso é útil quando se tem um valor constante nas fórmulas. Para trancar uma célula basta colocar um "$" antes da linha e coluna daquela célula na barra de fórmulas, isso pode ser feito utilizando o "F4" com o nome da célula selecionada.

*Célula trancada(Referencia absoluta)*
![[Pasted image 20250101193826.png]]

*Célula não trancada(Referencia Relativa)*
![[Pasted image 20250101193942.png]]

### Colar Especial

São diversas formas de colagem que o Excel disponibiliza, para acessa-lo é necessário copiar um texto> clicar com o botão direito> colar Especial e selecionar uma opção, ou, utilizar o botão de colagem na tela inicial.

Os tipos principais de colagem especial são:
a colagem normal;
a colagem somente das fórmulas(neste caso ele vai acompanhar a referencia);
A colagem das fórmulas e da formatação dos números;
A colagem mantendo a formatação original;
A colagem sem bordas;
A colagem mantendo a largura da coluna original;
A colagem transposta(neste caso ele transforma linhas em colunas e vice-versa);
A colagem somente de valores(cola o valor bruto, sem manter formulas ou formatação ), de valores e formatação de numero(cola o valor bruto mantendo a formatação original, mas não cola fórmulas) e valores e a formatação original(mantém a formatação do números e o estilo das células,  mas ao cola a fórmula);
A colagem somente da formatação, sem os valores;
A colagem com vínculo(cola os valores brutos mantendo vínculo com as células originais, ou seja, a mudança das originais ainda muda a colagem );
A colagem de imagem(transforma as células selecionadas em imagens) e a de imagem com vinculo(transforma as células selecionadas em imagens, mas mantem um vinculo com as originais, de forma que a mudança delas altere os valores na imagem).

No mais, é possível utilizar operações no colar Especial, assim ele cola os valores originais por cima dos outros valores de outra célula e executa alguma operação básica na colagem.
## Conceitos Intermediários

### Formatação Condicional

A formatação condicional é a estilização da célula baseado em uma condição. As regras de formatação e os tipos de formatação, são gerenciadas no botão "Formatação Condicional" na guia Inserir:

![[Pasted image 20250128031018.png]]

#### Regras de formatação
Para as regras de formatação, temos por padrão o Realce de células em condições gerais ou nos primeiros/últimos valores, ou seja, no primeiro as células serão realçadas caso: estejam entre dois valores, sejam maior menor ou igual a algum valor, sejam duplicados, entre outros.

![[Pasted image 20250128031727.png]]

Já no segundo, terão realce os 10 primeiros ou últimos valores, dentre outras regras

![[Pasted image 20250128031839.png]]

#### outros tipos de formatação

Há outros tipos de formatação além do realce de células, sendo os principais a Barra de dados e a Escala de cor.

O primeiro fara um preenchimento gradual das células proporcional ao valor inserido nelas:

![[Pasted image 20250128032426.png]]

![[Pasted image 20250128032446.png]]

Já o segundo fara um preenchimento gradiente das células proporcional ao valor nelas

![[Pasted image 20250128032622.png]]

![[Pasted image 20250128032717.png]]

Há mais dois pontos para se notas sobre a formatação condicional: 1º. A formatação condicional sobrepõe qualquer outra formatação na célula, ou seja, ela será a principal.
2º. Dependendo do tipo de formatação, elas pode se mesclar nas células. Por exemplo, se uma formatação muda o realce da célula, enquanto outra muda o tipo de dado, se uma célula atender as duas formatações então ela será realçada e terá o tipo de dado alterado.
#### Formatação Personalizada

Para abrir a caixa de personalização na formatação condicional, basta clicar em "Mais regras" em qualquer outra caixa de formatação, ou no botão "Nova regra", esta é a tela que aparecerá:

![[Pasted image 20250128034425.png]]

No primeiro campo temos o tipo de regra a ser aplicada, que não difere muito dos ja falados. Ja no campo de baixo temos a estilização da formatação, note-se que este campo muda de acordo com a regra selecionada e o tipo de formatação, seguem alguns exemplos:

![[Pasted image 20250128034825.png]]

![[Pasted image 20250128034852.png]]

![[Pasted image 20250128034913.png]]

As regras que mais serão utilizadas serão "Formatar Células que contenham" e "Formatar Células onde uma fórmula é verdadeira". Dentre os dois o ultimo é o mais complicado, pois deve ser utilizada uma formula e ela deve estar estritamente correta parar funcionar, ainda assim, as formulas não são necessariamente as do Excel, podendo ser uma comparação ou operação simples.


### Fórmulas de contagem

As fórmulas de contagem no Excel são feitas para contar linhas com algum conjunto de dados. Dentre as principais temos CONT.NÚM, CONT.VALORES, CONTAR.VAZIO.

Uma observação é que para cada fórmula é possível passar um único parâmetro, com este sendo uma matriz com todos os valores, ou passar vários parâmetros, com cada um deles sendo uma das colunas para contagem.
####  CONT.NÚM

A fórmula CONT.NÚM conta apenas células que contenham números, ou seja, células vazias ou com textos serão ignoradas.

CONT.NÚM(intervalo1; < Intervalo2 >; ...)

![[Pasted image 20250201100711.png]]

#### CONT.VALORES

A fórmula CONT.VALORES conta as células que contenham qualquer valor, ou seja, serão ignoradas apenas células em branco, desta forma até mesmo células com erro são contadas, diferente da CONT.NÚM.

CONT.VALORES(intervalo1; < Intervalo2 >; ...)

![[Pasted image 20250201100734.png]]
#### CONTAR.VAZIO

A fórmula CONTAR.VAZIO conta apenas células vazias, ou seja, células com qualquer valor serão ignoradas.

CONTAR.VAZIO(intervalo1; < Intervalo2 >; ...)

![[Pasted image 20250201100753.png]]
### fórmula SE

A fórmula se verifica se uma condição é verdadeira ou falsa e retorna algo dependendo do resultado lógico. Ela pode ser escrita junto das fórmulas E e OU para verificar mais de uma condição lógica e podem ser escritas outras funções SE uma dentro da outra, como se fosse um else IF.

Função SE: 
SE(condição; valor se verdadeiro; valor se falso)

Função se com E ou OU: 
SE(E/OU(valor lógico 1; valor logico2;..); valor se verdadeiro; valor se falso)

Função SE aninhada: 
SE(condição; valor verdadeiro;SE(condição; valor verdadeiro;..))

Já foi informado o uso das funções E e OU, mas em um geral, o primeiro retornará verdadeiro caso todas as condições sejam verdadeiras, caso contrário retornara falso; o segundo retornara verdadeiro se ao menos uma condição for verdadeira, e retornara falso se todas forem falsas.

E/OU(valor lógico 1; valor logico2;..)

No mais, a função SE possui outras variantes, como a SEERRO, onde a condição é se há um erro na célula, e os resultados são como a célula será tratada se o erro existir ou não.

### Autopreenchimento e reconhecimento de padrões

O Excel possui uma ferramenta de autopreenchimento, ela preenche automaticamente baseado em algumas listas prontas mas é possível criar uma lista personalizada para o preenchimento, e além disso o Excel pode reconhecer padrões de números quando se tem mais de uma célula numérica preenchida.

Para executar o autopreenchimento basta preencher uma ou mais células com algum valor e arrastar o canto da célula para algum lado e o Excel tentará encontrar um padrão para seguir, ao segurar CTRL no momento de arrastar, o Excel vai somar os números em uma progressão unitária ignorando os padrões que encontrar(Ou seja, vai somar de um em um ignorando os padrões) , ou ele vai copiar o mesmo texto da célula nas células seguintes.
Para criar uma lista personalizada de padrão basta seguir o caminho: Arquivo> configurações/opções> Avançado> Editar listas personalizadas.

Por fim, o Excel pode utilizar o reconhecimento de padrões para fazer separação nos textos, ele encontra um padrão nos textos das células adjacentes e verifica se eles podem ser separados, se puderem ele da a opção de seguir diretamente com o texto extraído:

![[Pasted image 20250111204811.png]]

Essa ferramenta também é chamada de preenchimento rápido

### Fórmulas de manipulação de textos

Uma das principais formas de juntar textos no Excel é utilizando o símbolo "&", igual é usado no Power BI, isso junta os textos de células esparsas em uma outra célula, é ainda possível utilizar isso em conjunto com um texto que já esta na célula, mas para isso o texto deve estar dentro de uma formula e deve ser colocado entre aspas. No fundo isso funciona como a concatenação de strings em alguma linguagem de programação:

![[Pasted image 20250111213058.png]]

Outra forma de fazer é utilizando a função CONCAT, funciona da mesma forma, mas os diferentes textos devem ser atribuídos como diferentes parâmetros na função:

![[Pasted image 20250111213303.png]]

No mais temos fórmulas de extração de texto (como DIREITA, ESQUERDA, EXT.TEXTO), e fórmulas de modificação de texto(Como MAIUSCULA, MINUSCULA, MUDAR).

Algumas formulas importantes são a de localização de caracteres, entre elas temos a fórmula LOCALIZAR e PROCURAR. 

#### LOCALIZAR


A função localizar encontra um texto específico dentro de uma cadeia de texto, e retorna a posição do caractere inicial do texto procurado, mas nao diferencia as letras maiusculas de minúsculas.

=LOCALIZAR(texto procurado; onde esta o texto procurado; < caractere de inicio de busca>)

Como está função retorna a posição inicial e um texto, é possível utiliza-la junto a fórmula SE ou a fórmula EXT.TEXTO. Ou alguma outra fórmula condicional onde se vá usar um texto como condição.

 Funcao procurar faz o mesmo da localizar, e pode ser usada nas mesmas opções, porem ela diferencia letras maiusculas de minúsculas.

![[Pasted image 20250120075533.png]]



### Gráficos

Os gráficos podem ser inclusos em juma planilha a partir da guia "inserir", aqui podem ser aplicados gráficos simples ou dinâmicos.

![[Pasted image 20250118174346.png]]

**Os gráficos comuns possuem três campos, O intervalo de dados do gráfico, as series do gráfico, e as categorias do gráfico. O intervalo de dados é a matriz de onde os dados serão retirados, as series são os valores dos gráficos e as categorias são as divisões do gráfico(Como se fossem as legendas).**

![[Pasted image 20250118174601.png]]

Ao criar um gráfico, ficam disponíveis as guias de Design e formatação do mesmo, na primeira é possível modificar os elementos do gráfico, seus estilos, ou a fonte de dados e tipo de gráfico.

![[Pasted image 20250118174802.png]]

Na área de formatação, é possível estilizar cada componente do gráfico, a mudança do componente é feita na caixa de seleção no canto superior esquerdo.

![[Pasted image 20250118175011.png]]

Cada gráfico possuem elementos diferentes para modificação, mas os principais são os títulos, rótulos de dados, e valores de série e coluna. A adição ou remoção de cada elemento é feita no campo "Adicionar elemento de gráfico".

![[Pasted image 20250118175149.png]]

#### gráficos dinâmicos

Os gráficos dinâmicos funcionam da mesma forma que uma tabela dinâmica, e eles permitem uma estruturação mais personalizada dos gráficos. Eles podem ser aplicados na guia "inserir"


Na sua criação são apresentados todos os conjuntos de dados do intervalo, e eles devem ser atribuídos para alguma das caixas disponíveis: Filtros, séries, categorias, ou valores. E fica disponível a guia de "*analise do gráfico dinâmico*", que permite a criação de segmentação de dados e linhas do tempo, a atualização e seleção de fonte de dados e a criação de formulas e relacionamentos. E ao se criar um gráfico dinâmico, é criada uma tabela dinâmica junto. As demais guias e funcionalidades continuam as mesmas.

![[Pasted image 20250118180958.png]]

![[Pasted image 20250118181014.png]]


### Fórmulas Avançadas

As principais fórmulas avançadas trabalham de maneira próxima com as condições e a busca em matrizes, são elas: PROCV, PROCH, PROCX, CONT.SE(S), SOMASE(S), MÉDIASE, e as fórmulas matriciais.

#### PROCV

A fórmula PROCV seleciona um dado em uma célula na coluna mais a esquerda de uma matriz, e depois retorna seu dado correspondente em X colunas a direita dela dentro da matriz. note-se que, a formula não trata da coluna inteira, apenas de uma parte selecionada, que é a matriz.

PROCV(dado de busca; Matriz de busca; Nº da coluna onde esta o dado correspondente; se a busca deve ser exata ou aproximada(0 ou 1)).

![[Pasted image 20250118181807.png]]

#### PROCH

Funciona da mesma forma que o PROCV, porem ao invés de procurar em colunas, a busca é feita em linhas, portanto ele Selecionará um dado na primeira linha da matriz e retornará outro da mesma coluna mas X linhas abaixo, contando a partir da primeira linha.

PROCH(dado de busca; Matriz de busca; Nº da linha onde esta o dado correspondente; se a busca deve ser exata ou aproximada(0 ou 1)).

![[Pasted image 20250118182030.png]]

#### PROCX

A função PROCX procura os valores valores correspondentes de uma matriz em outra matriz, e permite a personalização das mensagens de erro, da objetividade da procura, e do tipo de procura(Se será binário ou não).

Um ponto importante, o valor a ser procurado esta no parâmetro "matriz de busca", enquanto a possível resposta a este parâmetro esta em "Matriz de resposta", o que vai ser procurado em atriz de busca é definido em "Valor de busca".

PROCX(Valor de busca; matriz de busca; matriz de resposta; mensagem se não for encontrado; exatidão da pesquisa; tipo de pesquisa).

![[Pasted image 20250118182956.png]]


#### CONT.SE

A formula CONT.SE fará a contagem de certas linhas dada uma condição, esta pode ser definida em uma célula ou diretamente na fórmula, com o valor a ser considerado para contagem.

CONT.SE(Intervalo de conta; critério para a conta)

![[Pasted image 20250118183311.png]]

Ha uma variação desta formula chamada CONT.SES, ela permite a contagem se for atendida mais de uma condição

#### SOMASE

A função SOMASE somara os valores de um intervalo baseado em uma condição, esta pode ser definida em uma célula ou diretamente na fórmula.

SOMASE(Intervalo; CRITERIO; Intervalo de soma)

O ultimo parâmetro é opcional, sendo usado somente se o intervalo principal não contiver os valores para soma.

![[Pasted image 20250118183602.png]]

Ha uma variação desta formula chamada SOMASES, ela permite a Soma se for atendida mais de uma condição
#### MÉDIASE

Funciona da mesma forma que a SOMASE, inclusive com o parâmetro opcional, a diferencia é que a MÉDIASE retorna a média de um intervalo de valores.

MÉDIASE(Intervalo; CRITERIO; Intervalo de média)

![[Pasted image 20250118183816.png]]

### Fórmulas de data

As fórmulas de data permitem um gerenciamento e extração de informações de data. Dentre as principais funções nós temos a HOJE, AGORA, DIA, MÊS, ANO, DIA.DA.SEMANA, DATA. E para funções de Hora temos, HORA, MINUTO, SEGUNDO.

#### HOJE

A função HOJE retorna apenas a data atual do computador, ela não precisa de nenhum parâmetro para ser utilizada mas pode servir de parâmetro para outras funções de dada.

HOJE()

#### AGORA

A função Agora retorna a data e hora atuais do computador. Não precisa de nenhum parâmetro para uso mas pode ser usada de parâmetro para outras funções

#### DIA

A função dia extrai o dia de uma data. Precisa de uma data como parâmetro e esta data pode ser a função HOJE ou AGORA, visto que retornam datas.

DIA(Data) // DIA(HOJE())
#### MÊS

A função MÊS extrai o MÊS de uma data. Precisa de uma data como parâmetro e esta data pode ser a função HOJE ou AGORA, visto que retornam datas.

MÊS(Data) // MÊS(HOJE())

#### ANO

A função ANO extrai o ANO de uma data. Precisa de uma data como parâmetro e esta data pode ser a função HOJE ou AGORA, visto que retornam datas.

ANO(Data) // ANO(HOJE())

#### DATA

A função DATA monta uma data dado o dia, mês e ano. Pode ser usada em conjunto com as funções DIA, MÊS e ANO, e pode ser usada junto das funções HOJE e AGORA

DATA(ANO, MÊS, DIA) // DATA(ANO(HOJE()); MÊS(HOJE()); DIA(HOJE()) )

#### DIA.DA.SEMANA

O Excel reconhece cada dia da semana como um numero de um a sete, sendo um o domingo e sete o sábado, sendo assim, dia da semana retorna o índice do dia da semana, ou seja, se o dia da semana for segunda, retornará Dois, se for quarta, retornará Quatro, Se for domingo, retornara Um, ETC.

DIA.DA.SEMANA(DATA)

#### HORA, MINUTO E SEGUNDO

Retornam, respectivamente, a hora minuto ou segundo de uma dada hora, sendo assim precisam de uma hora de onde extrair os dados, e com isso podem ser usadas em conjunto com a função AGORA.

HORA, MINUTO, SEGUNDO(Hora)




### Filtros e Classificação

#### Filtros
Para fazer a aplicação de filtros no Excel, basta habilitar a opção na guia "Dados", ele por padrão aparecerá na primeira célula preenchida da coluna, e ele pode ser aplicado em varias células de uma vez ao selecionar varias células.

O filtro pode ser utilizado para isolar células ou podem ser utilizadas configurações especificas de filtro para cada tipo de dado. Por exemplo, quando é um numero você pode filtrar por "Maior/Menor Que", "Igual á", "Diferente De", etc. O mesmo vale para datas e textos, cada tipo de dado possuem configurações de filtros personalizadas que podem ser utilizadas.

OBS: Caso as células possuam paletas de cores, é possível filtrar por estas paletas

![[Pasted image 20250201131530.png]]

![[Pasted image 20250201131553.png]]

![[Pasted image 20250201131703.png]]

![[Pasted image 20250201131736.png]]

#### Classificação

Em suma, a classificação permite organizar os dados em ordem crescente ou decrescente, sua aplicação pode ser feita por meio do botão de filtro nas primeiras células da coluna, ou selecionando todo o conjunto de dados e clicando no botão de Classificar na guia "Dados".

![[Pasted image 20250201131530.png]]

Um ponto interessante sobre a classificação é que os dados adjacentes as células classificadas são alterados junto das células originais, ou seja, caso haja uma sequencia de números e adjacente a ela alguma outra informação, a outra informação mudará conforme a ordem dos números for alterada. Mas isso pode ser alterado selecionando o conjunto de dados e aplicando aclassificação no botão classificar na guia dados.


![[Pasted image 20250201132812.png]]

*Dados classificados em ordem crescente*
![[Pasted image 20250201132423.png]]

*Dados classificados em ordem Decrescente*

![[Pasted image 20250201132458.png]]

*dados classificados por cor*

![[Pasted image 20250201132548.png]]


## *Referencies*

[[Documentação Principal - Power Query]]