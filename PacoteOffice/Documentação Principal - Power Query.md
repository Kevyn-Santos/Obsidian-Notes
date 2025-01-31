Tags: #pacoteOffice

## **POWER QUERY**

O Power Query é uma ferramenta do Power BI que permite o tratamento dos dados antes destes serem importados para um uso mais complexo, é esta ferramenta que permite a exclusão ou inclusão de colunas e linhas, a mudança dos tipos de dados, a mesclagem de tabelas ou colunas, dentre outras coisas. Em suma, esta é a ferramenta que permitirá um tratamento inicial e fundamental dos dados que serão utilizados ao longo do relatório.

OBS: O Power Query do Power BI é o mesmo para o Excel.
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