# Introdução
O Pandas é um framework do python que permite a manipulação de dados de diversas fontes, como arquivos CSV, Excel, Sql, PDF, entre outros. Seu principal uso é tratar os dados para organiza-los e manipula-los, como fazer a criação, exclusão e renomeação de colunas e linhas, fazer a inclusão ou exclusão de informações e principalmente, fazer a leitura dos arquivos para permitir o uso de suas informações em gráficos ou outros meios. Conversa muito bem com bibliotecas como matplotlib, plotly e openpyxl.

# Nomenclaturas
Seguem algumas nomenclaturas do pandas:

Dataframe - Este é a tabela que esta sendo trabalhada, sendo assim pode ser chamado de Dataframe/Dataset/Tabela

Variáveis/atributos - são as colunas da tabela
Índices/iterações - são as linhas da tabela

Series - Array unidimensional que retorna os índices e as iterações de uma coluna ou linha especificas, ou seja, é uma serie de informações, podendo elas estarem em linhas ou colunas.

# Atribuição de valores
A atribuição de valores pode ser feita com uma constante ou uma variável, um valor constante seria um valor único para todas as iterações da coluna, enquanto um valor  variável seriam valores diferentes para cada iteração.

Para atribuir um valor constante a uma coluna, basta seleciona-la e atribuir o valor tal qual em uma lista.
DF["Coluna"] = Valor

Para atribuir um valor variavel, a quantidade de valores deve ser igual a quantidade de iterações da coluna, sendo assim é comum passar uma lista de valores neste caso.
DF["Coluna"] = Lista_de_valores 

A criação de colunas é feita como num dicionario, ou seja, nós paenas passamos um nome que não existe ainda e passamos os valores para ele.

DF["Coluna nova"] = novos valores/ lista/repetição/ uma coluna ja existente 