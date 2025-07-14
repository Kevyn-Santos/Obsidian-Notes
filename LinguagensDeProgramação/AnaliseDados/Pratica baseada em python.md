#AnaliseDados #programação 

[Python para analise de dados - Limpeza](https://wesmckinney.com/book/data-cleaning)

A biblioteca Pandas do python proporciona vários meios de fazer a coleta e limpeza dos dados, as principais funções, parâmetros e utilidades de cada uma serão descritos nesta secção.

# Coleta
[[Webscrapping]]
## Arquivos

## Banco de dados

## API


# Limpeza
## Valores faltantes:
Em python, a identificação de valores faltantes pode ser feita com a função *isna* (Ou *Isnull*, elas são iguais). Esta função retorna uma série booleana onde os valores ausentes(NAN || NA || NONE) são verdadeiros, fazendo assim o mapeamento dos valores. Após identificar os valores ausentes, eles podem ser deletados ou preenchidos utilizando as funções *Dropna* e *Fillna*.
Duas observações: 
*isna* pode ser usado com formulas estatísticas para calcular quantos valores nulos possuímos no DF por coluna(P.Ex. DF.isna().sum() -> Soma os valores faltantes no DF).
Como *isna* trata apenas valores *NAN ou NONE* como ausentes, outros valores como '-' ou 'missing' devem ser tratados de antemão e substituídos com a função *Replace* 

A função *Dropna* remove as linhas ou colunas que contenham valores nulos, criando uma cópia do DF original e alterando apenas a cópia. Por padrão, caso haja ao menos um valor nulo na linha ou coluna ela será deletada, mas há parâmetros específicos que podem modificar o funcionamento da função.
	**How** -> Contem os valores *any* e *all*. O primeiro exclui a linha/coluna caso haja ao menos um valor NA nela, o segundo faz a exclusão somente se todos os valores forem NA. 
	**Axis** -> 0 faz a exclusão de linhas; 1 faz a exclusão de colunas
	**Thresh** -> Define um limite mínimo de valores Não nulos que uma linha/coluna precisa ter para não ser excluída. ou seja: Thresh=3 -> a linha/coluna precisa de pelo menos três valores preenchidos para não ser excluída.

A função Fillna preenchera os dados vazios de diversas formas, as principais são:
	**Valor constante(Escala**r) -> Se for passado um único valor, então todos os valores ausentes serão substituídos por ele
	**Series/dict/Dataframe** -> Permite especificar um valor para cada linha/coluna do DF. Os valores não podem ser listas.
	**Method** -> possui os valores 'bfill' e 'ffill'. A principal diferença entre eles é que: dado um valor não nulo próximo de um NA. Com 'ffill' todos os valores NA a frente deste não nulo serão preenchidos com o valor dele, e com o 'bfill' o preenchimento será feito nos NA atrás dele. Em termos mais simples e grossos, ffill preenche todos os NA a frente de um numero com o valor daquele numero, e bfill faz o mesmo porem para os números que estão atrás.
	**Limit** -> Este parâmetro pode acompanhar o *method*, indicando quantas linhas/colunas de valores vazios devem ser preenchidos pelo parâmetro.
	**Estatísticas** -> Por fim, é possível utilizar estatísticas como média, mediana, desvio padrão, máximo, mínimo, etc. para preencher os valores vazios, bastando utilizar a formula correspondente dentro da função, por exemplo: *df[coluna].fillna(df['coluna'].mean/max/mín...)*
	Obs: Futuramente os métodos ffill e bfill serão substituídos por funções que  terão o mesmo nome

## valores duplicados
[Python para analise de dados - Limpeza](https://wesmckinney.com/book/data-cleaning)
[Python para analise de dados - Limpeza(Documentação Pandas)](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.duplicated.html)


A verificação de valores duplicados em python é feita com a função *Duplicated*, ela verifica se em um DF há um valor repetido, e retorna uma serie booleana indicando *true* onde há estes valores. 
Além dela temos a função *Drop_duplicates*, que retorna um novo DF sem os valores duplicados.
Ambas as funções possuem os parâmetros *subset* e *keep*:
*  O primeiro pode ser usado para definir a coluna a ser tratada/analisada no DF. 
* O segundo parâmetro marca quais valores não serão considerados duplicadas, ele tem as Keywords 'first', 'last', 'False; 
	* 'first' -> Trata as primeiras ocorrências como os valores únicos, e todas as repetições são consideradas duplicadas
	* 'last' -> trata as ultimas ocorrências como os valores únicos, e todas repetições são consideradas duplicadas
	*  False marca todos os valores como duplicados, com exceção das ocorrências que são totalmente únicas, sem nenhuma duplicidade no DF, geralmente linhas que aparecem somente uma vez.

Temos por exemplo: 
* DF.duplicated(subset=['Coluna1']) -> para verificar os valores duplicados da coluna 1
* DF.drop_duplicates(subset=['Coluna1']) -> para retirar os valores duplicados se baseando da coluna 1

Outros parâmetros da função Drop_duplicates são: Inplace(Que sobrescreve o DF original ao invés de criar uma cópia) e o Ignore_index(Que cria um novo índice para a cópia sem as duplicadas)

## Formatação dos dados
[Numpy DataTypes](https://www.w3schools.com/python/numpy/numpy_data_types.asp)
[Python para analise de dados - Conversão por mapeamento](https://wesmckinney.com/book/data-cleaning#prep_mapping_values)
[Python para analise de dados - Substituição de valores](https://wesmckinney.com/book/data-cleaning#prep_replace)
[Pandas Documentation - replace](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.replace.html)
[Pandas Documentation - rename](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.rename.html)


Uma das partes mais importantes em análise de dados é a normalização deles, ou seja, a padronização ou correção dos tipos de dados. Isso pode ser feito de varias formas diferentes.

* método *astype*:
	Este método do pandas permite modificar o tipo de dados de uma coluna, eles podem ser alterados para tipos padrão do python ou para outros tipos adicionados pelas bibliotecas numpy e pandas. por exemplo:  i/int(integer), f/float(float), b/bool(boolean), S/string(string), O(object), category(dados categóricos), datetime64(datas), etc.
	
	Outros pontos são:
	* A função pode receber um dicionário para mudar colunas especificas para tipos específicos.
	* Tipos de dados que não puderem ser convertidos(P.Ex letras-> int) retornarão erros

* Mapeamento
	Os dados podem ser modificados ou organizados utilizando, principalmente, a função *map*, esta recebe uma outra função ou dicionário e modifica uma *series* baseado nisso. P.ex. dado o seguinte código:
	
	data = pd.DataFrame({"food": [
				"bacon", "pulled pork", "bacon", 
				"pastrami", "corned beef", "bacon", 
				"pastrami", "honey ham", "nova lox"],
    "ounces": [4, 3, 12, 6, 7.5, 8, 3, 5, 6]})
    
	animal = {
    'bacon': 'pig',
    "pulled pork": "pig",
    "pastrami": "cow",
    "corned beef": "cow",
    "honey ham": "pig",
    "nova lox": "salmon"
	}
	data['animalCorresp'] = data['food'].map(animal)
	
	O DF retorna uma serie de alimentos, mas não possui o animal correspondente a ele. O dicionário 'animal', contém os alimentos com os animais relacionados. A função map atribuirá para cada comida em *data['food']* o animal correspondente indicado no dicionário 'animal', criando uma nova coluna chamada *animalCorresp*.
	
	Além disso, no código acima todos os alimentos não estão capitalizados, poderíamos adicionar a seguinte função ao código para resolver isso:
	
	def maiuscula(str):
	    return str.capitalize()
	
	A aplicação dessa função no DF também pode ser feita com *map*:
	
	data['food'] = data['food'].map(maiuscula)
	
	Assim capitalizando todas as iterações na coluna *food*.
	Por fim, Map pode receber Funções Lambda.

* Substituição de valores com *replace*
	A função replace substitui valores de maneira mais direta dentro de um DF. É possível substituir os valores um a um, substituir uma lista de valores por um valor, substituir uma lista de valores por outra lista, ou passar um dicionário que indica qual valor deve ser substituído pelo que:
	
	df.replace(987, np.nan) -> substitui o valor 987 por NAN
	df.replace([987; 1000], np.nan) -> substitui o valor 987 e 1000 por NAN
	df.replace([-999, -1000], [np.nan, 0]
	df.replace({-999: np.nan, -1000: 500})
	
	Além disso a função possui os parâmetros:
	Inplace -> Modifica o DF original ao invés de criar uma cópia
	regex -> permite substituir caracteres de expressões regulares

* Modificação de títulos de índices e colunas com *rename*
	Índices e colunas podem ser modificados com Map(*df.index/columns.map()*), mas outra opção é utilizar a função *rename*. Ela é utilizada principalmente com dicionários, mas também pode ser utilizada com alguns parâmetros e retorna uma cópia do DF original.:
		**Modificação por dicionários:** É passado um dicionário com os valores antigos e os novos, por padrão o dicionário vai modificar primeiro as linhas, então caso queira mudar as colunas é preciso utilizar junto o parâmetro *axis=1*. 
		P.EX.: df.rename({'nomeColuna1': 'NovoNomeColuna1'}, axis=1)
		**modificação por indicação direta:** Ao invés de utilizar somente dicionários, é possível aplicar as modificações para as linhas ou colunas diretamente utilizando os parâmetros *index* e *columns*. Eles são o equivalente á *axis=0 e axis=1*. um exemplo de modificação é: 
		df.rename(index={'NomeLinha1': 'novo_nome_linha1'}, columns={'NomeColuna1':*novo_nome_Coluna1*}).
	
	Além disso, a função *rename* tem os parâmetros *Inplace*(Para modificar o DF original), *level*(Em caso de multindexação, modifica somente os rótulos de níveis específicos), *erros*(define se os erros na renomeação serão mostrados(*raise*) ou não(*ignore*))

* Uso das fórmulas *to_datetime*, *to_timedelta*, *to_numeric*


# Visualização

[Seaborn Tutorial](https://www.youtube.com/watch?v=6GUZXDef2U0)
[matplotlib Tutorial](https://www.youtube.com/watch?v=wB9C0Mz9gSo)


## Matplotlib

### Importação:
utilizamos na construção dos gráficos o módulo pyplot do matplotlib, portanto a importação da biblioteca é feita da seguinte forma: import matplotlib.pyplot as plt.

### Estrutura dos gráficos:

Existem diversos gráficos no matplotlib e com vários elementos entre eles, ha na documentação a seguinte imagem mostrando a anatomia dos gráficos

![[Pasted image 20250714083240.png]]

Mas algumas funções importantes dos elementos são:
plt.title('') -> coloca um titulo no gráfico
plt.xlabels() -> coloca um rótulo no eixo X
plt.ylabels() -> coloca um rótulo no eixo Y

### Tipos de gráficos:

* Linha -> cria um gráfico de linha simples a partir de um array de valores
	* código: Plt.plot(array)
	* ![[GráficoLinha.png]]

* Barra -> cria um gráfico de barras simples a partir de dois arrays, um para X e o outro para Y
	* código: plt.bar(x=array, height=array) -> height é a altura do gráfico, então os valores de Y
	* ![[GráficoBarra.png]]

* 
## Seaborn

