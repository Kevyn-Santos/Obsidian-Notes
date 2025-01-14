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
A colagem somente de valores(cola o valor bruto, sem manter formulas ou formatação ), de valores e formatação de numero(cola o valor bruto mantendo a formatação original, mas não cola fórmulas) e valores e a formatação original(mantém a formatação do numeros eo estilo das células,  mas ao cola a fórmula);
A colagem somente da formatação, sem os valores;
A colagem com vínculo(cola os valores brutos mantendo vínculo com as células originais, ou seja, a mudança das originais ainda muda a colagem );
A colagem de imagem(transforma as células selecionadas em imagens) e a de imagem com vinculo(transforma as células selecinadas m imagens, mas mantem um vinculo com as originais, de forma que a mudanca delas altere os valores na imagem).

No mais, é possível utilizar operações no colar Especial, assim ele cola os valores originais por cima dos outros valores de outra célula e executa alguma operação básica na colagem.

## Conceitos Intermediários

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

### formatação condicional


### funções de data



### filtros, classificação, validação de dados e definição de nomes


### gráficos 


### fórmulas avançadas 


### Outros



## conceitos avançados

### Tabelas Dinâmicas



### Trabalho com metas


### Macros e VBA


### Power Query

