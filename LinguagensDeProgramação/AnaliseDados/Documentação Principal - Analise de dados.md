#AnaliseDados #programação 

[Caminhos na carreira de análise de dados](https://roadmap.sh/data-analyst/career-path)
[[Análise exploratória de dados(EDA)]]
[[Data Mining]]


## O que é analise de dados

Analise de dados são os processos de transformar dados em informações mais uteis e intuitivas(seja como gráficos, dashboards ou modelos preditivos) que vão auxiliar a empresa na tomada de decisão. 
Isso é feito pelo uso de técnicas de analise como limpeza de dados, extração de estatísticas e visualização dos dados. 

Em suma, é saber como pegar os dados brutos de uma empresa e transforma-los em algo que auxilie na tomada de decisões futuras a partir de padrões ou tendencias, para isso o analista precisa ter a habilidade de olhar para o passado, interpreta-los no presente e dizer o que pode acontecer e o que pode ser feito no futuro. Isso é feito com diversas técnicas, inclusive, com aprendizado de maquina em analises mais avançadas.

Um ponto importante: a analise de dados é a junção de habilidades técnicas com o modelo de negócios, contexto ou setor de uma empresa. Ou seja, você precisa saber como aquele ramo empresarial atua. Por exemplo, se você for um analista de dados bancários, você vai encarar os dados de uma maneira, mas se for um analista de dados industrial, sua percepção será outra. Então saber como funciona o tipo de negocio que você vai entrar é tão importante quanto saber como limpar dados e transforma-los em relatórios.

## Quais os tipos de analise de dados

[Os quatro tipos de análise de dados](https://careerfoundry.com/en/blog/data-analytics/different-types-of-data-analysis/#descriptive-analytics-what-happened)

São quatro os principais tipos de analise de dados: Descritiva, Diagnostica, Preditiva e Prescritiva, em resumo elas tratam do que aconteceu, porque aconteceu, o que pode acontecer e o que pode ser feito.

### Análise descritiva:

[O que é análise descritiva](https://careerfoundry.com/en/blog/data-analytics/descriptive-analytics/)

O foco deste tipo de análise é descrever o que aconteceu, ou seja, ela resume(sumariza) e exibe os dados, isso é feito após o pré-processamento dos dados(coleta e limpeza), principalmente com a técnica de **agregação de dados**.

A agregação busca apresentar os dados de maneira resumida, mas sem muito detalhe, é como se ela mostrasse as estatísticas mais básicas de um conjunto de dados.

Há também a [[Data Mining |Mineração de dados]], ela pode se apoiar na analise descritiva, porem busca algo mais detalhado e robusto, transformando as tendencias e padrões dos dados brutos em gráficos e dashboards, portanto ela é mais associada a analises diagnosticas e preditivas, por conta disso, um estudo mais profundo dessa técnica é necessário.

Em geral, a analise descritiva trata do resumo dos dados, extraindo estatísticas, os sumarizando e os aplicando em dashboards, indicadores e KPI's. Ou seja, ela trabalha tanto com o tratamento e limpeza de dados quanto com a visualização deles.

#### Aprofundamento:

No fundo, a analise descritiva segmenta os conjuntos de dados em pedaços menores, extraindo e resumindo suas características e pontos mais importantes, por isso de seu nome, pois o foco principal é contar o que aconteceu a partir do uso de estatísticas básicas como, medidas de distribuição(frequência ou contagem), tendencias centrais(moda, media e mediana), variações(Desvio padrão e variância), quartis e porcentagens, sem se preocupar em como ou porque aconteceu. Essa extração de estatísticas pode ser feita em ferramentas como Python(pandas), R(Dplyr), Excel, etc.

Ou seja, ela é o ponto de partida para uma analise mais profunda, como a diagnostica ou a preditiva e, ainda assim, serve bem para diversos tipos de analises, por exemplo, financias, trafego em sites, pesquisas, vendas, etc. A exibição dessas estatísticas é geralmente feia por meio de gráficos(Histograma, linha, pizza, barra, caixa, etc.) ou tabelas dinâmicas, em ferramentas como Python(matplotlib/seaborn, plotly, etc.), R(Ggplot2) Excel, PowerBi, Tableau, etc. 

Neste ponto fica evidente que a analise descritiva providencia uma visão intuitiva e direta dos dados coletados, focando nos pontos chave, sendo bem simples de trabalhar, pois, utiliza apenas matemática estatística básica no seu funcionamento, entretanto, analises mais profundas e replicáveis, que expliquem porque e como algo aconteceu, ou, o que pode acontecer, não podem ser feitas com ela, sendo necessário o uso das analises diagnostica e preditiva para tal.

OBS: Será necessário aprender os conceitos e usos de estatística básica, principalmente em medidas de distribuição, tendencias centrais, variâncias e quartis.
### Análise diagnostica:

[O que é análise Diagnostica - HBS](https://online.hbs.edu/blog/post/diagnostic-analytics)
[Análise Diagnostica - o que é, técnicas e desafios](https://www.thoughtspot.com/data-trends/analytics/diagnostic-analytics?utm_source=chatgpt.com)

O objetivo dela é entender porque as coisas aconteceram, isso é feito analisando anomalias, tendencias, e padrões nos seus dados, ou seja, discrepâncias, valores muito baixos, valores muito altos, correlações, causas prováveis, entre outros. neste ponto o analista busca fontes adjacentes de dados que podem ajudar a explicar essas anomalias, como a demora em um processo bancário, uma taxa de juros muito alta ou muito baixa ou mesmo a opinião publica sobre o produto ou empresa. Em outras palavras, como o nome sugere isso é um diagnóstico, ou seja, você vai entender a causa de um problema pelos seus efeitos, como se estivesse andando do final para o começo, e este começo é a causa raiz.

Num geral, a análise descritiva retorna os dados tratados, esses dados apresentam valores muito discrepantes ou incomuns, e a analise diagnostica busca entender porque estes valores apareceram, buscando a causa raiz deles.

#### Aprofundamento:


Existem três técnicas principais na análise diagnostica dos dados, sendo elas:

* **Teste de hipóteses:**
	 O teste de hipótese é uma técnica onde se supõe algo sobre os dados e tentamos provar se essa suposição esta certa ou errada utilizando testes estatísticos. Geralmente esta suposição é feita com algo no passado ao invés do futuro, pois no ultimo caso estamos tratando da analise preditiva(P.ex. As vendas caíram por uma aumento dos preços, ao invés de, as vendas vão cair se os preços subirem mais). Com o teste de hipóteses podemos averiguar se algo ocorreu ao acaso ou se há uma causa mais especifica.

* **Analise de correlação e causa:**
	A analise de correlação busca verificar se uma variável esta relacionada a a outra, se uma influencia diretamente a outra, e se essa é a cauda daquela. As variáveis relacionadas podem mudar de maneira proporcional ou inversamente proporcional a outra, mas não significa que uma é necessariamente a causa da outra. 
	Um exemplo mais visual seria, duas variáveis são como duas varetas ligadas por uma corda, o movimento de uma vareta influencia a outra, porem o movimento da primeira pode não ser a causa principal do movimento da segunda, na verdade, ambas as varetas podem estar ligadas a uma terceira, e este é a causa raiz da movimentação das outras duas.

* **Análise de regressão:**
	Em resumo, a análise de regressão verifica a interação de duas ou mais variáveis ao longo do tempo, averiguando como uma influencia a outra para determinar de maneira mais precisa as causas de algum acontecimento. Essa analise pode ser feita manualmente ou podemos usar *machine learning* para treinar um modelo que realize esta análise(com Scikit learn, por exemplo).

### Análise preditiva:

Ela busca prever o que pode acontecer baseando-se nas tendencias e padrões encontrados nas analises descritivas e diagnósticas, podendo ser utilizada não só para prever eventos futuros mas para classificar acontecimentos se baseando no comportamento de algo ao longo do tempo. Note-se que ela não é 100% precisa, mas ela pode dar boas aproximações.

Por exemplo, a analise descritiva viu que um cliente compra mais coisas no meio do ano e menos no final, a analise diagnostica viu que isso é por uma pequena alta no valor guardado no meio do ano e uma queda significativa no final, a analise preditiva vai dizer se essa pessoa seguira este padrão ou não, e com isso, se vale a pena dar um empréstimo a ela no final do ano, classificando ela em alguma faixa de cliente baseado no empréstimo que pode ser proposto.

Este tipo de analise pode ser feito por um humano mas é possível treinar um algoritmo para identificar estes padrões e dar respostas cada vez mais precisas, isto é o machine learning. Mas além dele, é possível utilizar técnicas mais clássicas, como modelos estatísticos e analises de séries temporais

### Análise prescritiva:

Ela visualiza o que aconteceu, porque aconteceu, o que pode acontecer e propõe as melhores ações nestes casos. Ela seria a mais complexa por tratar de modelos de machine learning, algoritmos estatísticos e todos os possíveis desdobramentos que um conjunto de ações pode ter.

por exemplo, o cliente realmente comprou mais produtos neste meio do ano, o que pode ser feito agora? a partir da analise de outros dados bancários um algoritmo pode dizer que é melhor dar um empréstimo de R$500 reais, pois é mais provável o cliente pagar ele em três meses do que pagar um empréstimo de R$1000 em seis meses.

Em suma, a analise prescritiva vai verificar todos os possíveis cenários de ação e escolher os melhores como guia para a decisão de uma empresa, seja simulando cenários, verificando custo X beneficio dessa ação, entre outras técnicas, enquanto segue as regras e parâmetros da empresa.

### Como elas se relacionam:

Em suma a relação entre os tipos de análise de dados é feito no seguinte fluxo:

**Analise descritiva**(verifica o que aconteceu,) -> **Analise diagnostica**(busca o porque dos acontecimentos terem ocorrido desse jeito, quais os padrões e quais as tendencias) -> **Analise preditiva**(Busca responder se um certo padrão vai se repetir ou não se baseando no que ocorreu)-> **Analise prescritiva**(busca os melhores cursos de ação baseado no contexto geral adquirido com as outras analises).

Um ponto importante é que nem todas elas são utilizadas a depender do projeto, e elas não precisam necessariamente seguir o fluxo apresentado. Além disso, o grau de dificuldade da análise sobe em cada tipo, com a analise descritiva sendo a mais simples e a análise prescritiva a mais complexa.



## Quais os conceitos chave da analise de dados:
[[Pratica baseada em python]]

Os principais conceitos em análise de dados são: Coleta, Limpeza, Exploração e visualização de dados. Cada um terá suas técnicas próprias e ramificações, mas tratemos por partes. A ideia é obter um Panorama geral do que cada conceito trata, para que desta forma seja possível entender o que se faz em cada parte e o que deve ser considerado em cada uma.

### Coleta:

[Coleta de dados](https://www.simplilearn.com/what-is-data-collection-article#what_is_data_collection)
[Métodos de coleta de dados](https://www.questionpro.com/blog/data-collection-methods/#What_are_Data_Collection_Methods)
[[Webscrapping]]

Essa é a parte mais importante, pois daqui virão os dados brutos que serão tratados e analisados. A coleta de dados pode ser feita a partir de arquivos no sistema(como uma planilha de Excel ou arquivo JSON), Bancos de dados, API's, Webscrapping entre outros. 

Os dados podem ser divididos em dois tipos:
* **Dados Quantitativos:** são números e estatísticas brutas de algum tipo de dado. 
* **Dados Qualitativos:** são as características do que esta sendo analisado. 

Por exemplo, em uma população de pessoas podemos verificar as seguintes características: Tamanho, idade, cor do cabelo, dos olhos e da pele, esses são os dados Qualitativos. 
Dentre esses dados teremos diversos números e estatísticas para cada registro, como a idade e altura de cada pessoa, quantidade de pessoas com certa cor de olhos, pele ou cabelo, esses são os dados Quantitativos.

Sendo assim, não é viável pegar todo tipo de dado existente para uma analise, por conta da abrangência e quantidade, então é necessário verificar algumas coisas antes de começar a coleta, são elas: 
* O propósito e objetivo da coleta dos dados(Que se liga ao objetivo da análise como um todo)
* Os tipos de dados que se deseja adquirir
* Quais métodos e técnicas serão utilizados na coleta, armazenamento e processamento dos dados.

#### Tipos de métodos de coleta de dados:

Existem dois métodos principais de coleta de dados: A coleta de dados primários(Fontes primarias), e a coleta de dados secundários(Fontes secundarias). 

O primeiro tipo trata da *Coleta de fontes primarias*, diretamente dos respondentes, o que pode auxiliar em uma resposta mais direta na analise. Este tipo de coleta pode ser feito por meio de:
* Pesquisas e questionários(Seja presencial ou online)
* Entrevistas(Que podem ser mais rígidas, com perguntas prontas, ou dinâmicas, como num bate papo)
* Observação(Observar o comportamento do que será analisado no ambiente natural daquilo)
* Experimentos(Fazer experimentos controlados para verificar as relações de causa e efeito)
* Grupos de foco(Incentivar um pequeno grupo a discutir sobre algo e coletar os dados da discussão)

O Segundo tipo de coleta trata da *Coleta de fontes secundarias*(ou, *análise secundária de dados*), ou seja, a análise é feita sobre uma pesquisa já realizada mas com um intuito diferente. Esse tipo de coleta pode ser feito por meio de:
* Fontes publicadas(Como livros, artigos, revistas, registros do governo, etc)
* Bancos de dados online
* Registros governamentais ou institucionais(Como de sites públicos do governo ou de ONG's)
* Dados de plataformas publicas(Como de redes sociais, sites, e indivíduos, grupos ou organizações publicas)
* Estudos e pesquisas antigas

Dentre estes métodos, a coleta pode ser feita a partir de analises mais cientificas e behavioristas, como completar frases e palavras e verificar como alguém agiria em uma situação, ou de maneira mais geral, com pesquisas pessoais, online ou por telefone.

Em geral, técnicas como observação, entrevistas e grupos focais tendem a gerar **dados qualitativos**, enquanto questionários e pesquisas estruturadas costumam gerar **dados quantitativos**. No entanto, muitos métodos podem gerar **dados mistos**, dependendo de como são conduzidos e qual o objetivo da pesquisa.

Por fim, os principais objetivos nesses métodos são:
* Garantir a integridade, validação, reprodução e relevância dos dados
* Alcançar os objetivos originais da pesquisa
* Garantir a validação e confiabilidade da pesquisa
* Auxiliar na tomada de decisão baseada nos dados coletados

#### Cuidados na coleta e integridade dos dados:

A coleta dos dados deve ser feita com os métodos certos para se evitar erros, imprecisões e irrelevância dos dados coletados, o que dificultaria ou prejudicaria a análise num geral, levando a conclusões errôneas, danos ao publico(Devido as medidas tomadas pela analise), e a incapacidade do estudo ser replicado e validado. Por isso é necessário utilizar as técnicas certas na coleta dos dados e se preocupar com a integridade deles.

A integridade dos dados pode ser verificada com um controle e garantia de qualidade bem formadas, ou seja, ela pode ser melhor atingida por meio de supervisão, comunicação e verificação constante de quem esta coletando os dados e como esta sendo feita a coleta, e por meio de guias, manuais e procedimentos bem estruturados que discorram com clareza sobre as técnicas que serão utilizadas em quais sujeitos de pesquisa, ou quais fontes de dados serão abordados na coleta(como banco de dados ou webscrapping). 

#### Ferramentas para coleta de dados:

Por fim, as ferramentas podem variar de acordo com a coleta que esta sendo feita. Uma abordagem mais clássica é fazer observações e pesquisas de campo, mas em termos mais atuais, utilizam-se ferramentas como:

##### 📝 **Ferramentas para coleta ativa (pesquisa/entrevistas):**

- **Google Forms, Microsoft Forms, SurveyMonkey** – criação de formulários online.
    
- **Google Meet, Microsoft Teams, Zoom** – realização de entrevistas virtuais (com possibilidade de gravação e transcrição).
    

##### 📊 **Ferramentas para organização e entrada manual:**

- **Excel, Google Sheets** – planilhas para entrada, limpeza e visualização inicial dos dados.
    

##### 🌐 **Ferramentas para coleta automatizada (web scraping / APIs):**

- **`requests`** – faz requisições HTTP para obter o HTML das páginas.
    
- **`BeautifulSoup`** – biblioteca de parsing de HTML/XML.
    
- **`Selenium`** – simula interações em páginas dinâmicas (JavaScript).
    
- **`Scrapy`** – framework de scraping mais robusto e performático.
    

##### 💾 **Coleta em bases de dados estruturadas:**

- **SQL (MySQL, PostgreSQL, SQLite)** – linguagem para consultar e extrair dados de bancos relacionais.
    
- **`sqlalchemy`, `sqlite3`** – interfaces Python para lidar com SQL.
    

##### 🐍 **Leitura e ingestão de arquivos com Python:**

- **`pandas`** – leitura de arquivos CSV, Excel, JSON, SQL, etc.
    
- **`polars`** – alternativa ao pandas, mais rápida e eficiente com grandes volumes de dados.

### Limpeza:
[O que é e como fazer Limpeza de dados](https://www.tableau.com/learn/articles/what-is-data-cleaning#:~:text=tools%20and%20software-,What%20is%20data%20cleaning%3F,to%20be%20duplicated%20or%20mislabeled.)
[[Pratica baseada em python]]

A limpeza de dados consiste principalmente no tratamento de quatro coisas: Dados faltantes, dados duplicados, Dados atípicos(muito fora da média), e dados no formato incorreto. Ou seja, é corrigir ou remover dados incompletos, mal formatados, corrompidos, duplicados ou muito extremos. O processo varia entre as bases de dados, e a aplicação prática da limpeza muda dependendo da ferramenta(por exemplo, a limpeza será feita com um conjunto de fórmulas no python, mas será feita de outra forma no Excel), mas há um caminho que pode ser seguido no tratamento deles:

1. **[[Pratica baseada em python#valores duplicados|Remover valores duplicados ou irrelevantes]]**
	Quando os dados vem de diversas fontes ou departamentos eles podem estar duplicados, desta forma avaliaremos se estes dados serão utilizados ou se devem ser removidos para uma análise mais precisa.
	
	Outro ponto é a remoção de dados irrelevantes, pois, as análises não serão feitas no conjunto todo, geralmente se deseja responder um número limitado de questões com cenários ou agentes específicos, portanto, a remoção de qualquer coisa fora deste escopo tornará a analise mais eficiente.
	
	Por exemplo, se deseja verificar quais clientes compraram um produto X no primeiro trimestre dos últimos três anos, mas a base contem vendas de todos meses dos últimos três anos. Desta forma será necessário excluir todos os trimestres com exceção do primeiro para esta análise, e será necessário remover qualquer venda duplicada do produto X, pois se quer somente os clientes que compraram aquele produto, não quantas vezes eles compraram.

2. **[[Pratica baseada em python#Formatação dos dados|Corrigir erros estruturais]]**
	Corrigir erros nos dados para que fiquem consistentes e num padrão, por exemplo: 
	* Nomenclatura(Nomes duplicados ou fora do escopo do conjunto de dados)
	* Capitalização e grafia(P.ex. 'Produto' e 'Produto' ou 'VenDa 1', 'VEnda2', etc.)
	* Classificação()
	* Tipos de dados inválidos(Numéros ou datas como Strings, Números no formato incorreto, etc.)

3. **[[Pratica baseada em python|Remover valores atípicos(Outliers) indesejados]]**
	Em primeiro lugar, um valor atípico é aquele muito disperso do resto dos dados ou da média deles. Por exemplo, temos três clientes, cada um tem os valores 1,2 e 3, é colocado na conta um quarto cliente, mas seu valor é 7. Este quarto cliente é um valor atípico.
	
	Algumas vezes os dados podem mostrar estes valores muito discrepantes ou que não fazem parte do escopo trabalhado, se esses dados atípicos forem um problema para o que esta sendo analisado eles podem ser removidos, mas isso depende do objetivo do projeto, pois você pode estar procurando esses valores atípicos.
	Por exemplo, dos clientes que compraram o produto X, a empresa deseja aqueles que mais gastaram dinheiro no produto. Se for calculada uma média ela vai ficar muito alta devido a um alto gasto de algumas pessoas, esses valores mais altos são os valores atípicos(Outliers) desejados pela empresa.
	
	Métodos como **boxplot, desvio padrão, z-score** ou **IQR (intervalo interquartil)** são usados para detectar esses valores.

4. **[[Pratica baseada em python#Valores faltantes|Lidar com dados faltantes]]**
	Há varias formas de lidar com dados faltantes, visto que vários algoritmos não aceitam dados faltantes, mas nenhuma é perfeita, pois isso prejudicaria a integridade dos dados. As duas principais opções são: 
	* Remover os dados - Geralmente quando faltam poucos
	* Substitui-los por outras observações(P.ex. Média, Mediana, Valores frequentes, Próximos valores ou valores anteriores). - Geralmente quando faltam muitos

5. **Validação**
	Após a limpeza será possível verificar se: 
	* Os dados fazem sentido
	* Se eles estão alinhados com o campo de trabalho
	* Se eles podem trazer ideias e auxilio para o trabalho
	* Se eles podem ajudar no desenvolvimento das próximas teorias. 
	
	Caso algo falhe, será possível verificar se é por conta de dados ruins ou uma limpeza mal feita.

#### Conclusão
Uma forma de verificar se um conjunto de dados é bom é a partir de uma análise sobre:

* A validade dos dados - Se eles são alinhados com as regras ou modelo de negócios da empresa

* A precisão dos dados - Se eles representam o mais próximo possível os eventos ou entidades reais analisados

* A completude dos dados - Se os dados necessários são todos conhecidos e estão presentes

* A consistência dos dados - Se os dados mantem consistência em todos os sistemas e fontes 

* A exclusividade e confiabilidade dos dados - Se os dados são únicos e vem de fontes confiáveis

* A atualização dos dados - Se os dados estão o mais atualizados quanto possível.

Em resumo, é possível verificar se um dado é bom se ele: Vir de fontes confiáveis, estar atualizado, manter a consistência e unicidade, for preciso com as entidades reais e estiver alinhado com o modelo de negócios.


### Exploração:
[Exploração de dados](https://www.heavy.ai/learn/data-exploration)

#### Introdução:

A exploração de dados é o primeiro passo para efetivamente conseguir informações uteis de um conjunto de dados. Ela usa técnicas estatísticas ou de visualização para extrair pontos como relações entre variáveis, valores discrepantes, tamanho, quantidade, precisão e distribuição dos dados. 

Um ponto importante é que os dados precisam estar limpos e padronizados antes de iniciar a exploração, pois assim as informações adquiridas se tornam mais precisas e corretas. 

Esta exploração pode ser feita manualmente ou de forma automatizada com aprendizado de maquina.
#### Análise Manual:

A exploração manual dos dados pode ser feita com diversas ferramentas e de diversos modos, desde a criação de Scripts em Python ou R, até a exploração utilizando as planilhas e fórmulas do Excel, com cada ferramenta possuindo um conjunto de fórmulas e técnicas próprias para auxiliar na exploração de dados.

É importante notar que a exploração não se resume somente a números e tabelas, mas tem um forte teor visual, pois é mais simples coletar e expressar as informações dos dados utilizando gráficos e imagens. 
Isso também permite identificar anomalias e discrepâncias nos dados que poderiam passar desapercebidas em uma tabela, portanto o uso de componentes visuais(como gráficos de barras, Histograma, dispersão, linha, etc.) é tão util quanto o calculo de estatísticas brutas.

#### Analise Automática:

A exploração automática de dados é feita principalmente com aprendizado de máquina, porem, os dados precisam estar bem tratados e validados antes de serem inclusos em um algoritmo deste tipo, visto que ele consumira os dados e, se eles não estiverem bem tratados, o algoritmo pode apresentar erros, tanto no código quanto nos resultados. por isso é importante fazer um pré-processamento e validação dos dados. Para isso, a fonte recomenda estes passos:

* Identificar o papel de cada variável no Dataset
* Realizar as analises Uni variada ou Bivariada
* Detectar e tratar valores ausentes ou discrepantes
##### Analises Uni Variada, bi variada e Multi Variada:
[Analises de variáveis](https://alexandreramos.blogs.sapo.pt/7901.html)

A analise uni variada é a aplicação de métodos estatísticos descritivos e inferenciais em cada variável separadamente. Ou seja, serão analisadas as variáveis uma a uma, sendo que elas não influenciam diretamente umas as outras. Pode-se ter como exemplo de analise uni Variada os cálculos de moda, média, mediana, variância, etc.

A analise bi variada é a aplicação de métodos estatísticos em duas variáveis, podendo ou não traçar uma relação de causa e efeito entre elas. Alguns exemplos de calculous aplicáveis a duas variáveis são: 
**[[Regressão linear]]:**
**teste qui-quadrado**
**correlação linear de Pearson ou Spearman**.

A analise multi variada é a aplicação de métodos analíticos em três ou mais variáveis dependentes e/ou independentes, podendo ou não ser traçada uma relação de causa e efeito entre elas, sendo que neste tipo, os indivíduos caracterizados com duas ou mais variáveis também podem ser analisados por estes métodos. Apenas estes métodos multivariados permitem analisar como múltiplas variáveis interagem, se relacionam e se influenciam. Alguns dos métodos deste tipo de analise são: 

**Análise de Componentes Principais (PCA)**
	Reduz a dimensionalidade de um conjunto de dados, transformando um conjunto de variáveis correlacionadas em um conjunto de variáveis não correlacionadas chamadas componentes principais

**Análise de Agrupamento (Cluster Analysis)**
	Agrupa observações em clusters com base em suas semelhanças, permitindo identificar grupos distintos dentro dos dados

**Análise Fatorial**
	Reduz um grande número de variáveis em um número menor de fatores latentes, que representam as dimensões subjacentes dos dados.

**Regressão Múltipla**
	Estima a relação entre uma variável dependente e múltiplas variáveis independentes, permitindo previsões e análises de impacto.

**Análise Discriminante**
	Classifica observações em grupos pré-definidos com base em um conjunto de variáveis, auxiliando na identificação de critérios de diferenciação entre os grupos.
#### Linguagens de programação utilizadas na exploração de dados:

As duas principais linguagens utilizadas na exploração dos dados são Python e R, ambas são bem flexíveis mas python geralmente é mais utilizado em Aprendizado de máquina enquanto R é mais utilizado em cálculos estatísticos, entretanto, o uso de uma ou outra depende do projeto e da empresa. 
As principais bibliotecas utilizadas em python para exploração e visualização de dados são o Pandas e matplotlib, enquanto a linguagem R ja foi criada com o intuito de realizar análises estatísticas, possuindo dentro de si o necessário para manipular os conjuntos de dados e construir visualizações com eles.

#### Menção: Descoberta de dados e Ferramentas de BI

Enquanto a exploração de dados coleta as maiores informações de um conjunto de dados, a descoberta de dados coleta informações relevantes para o negocio neste conjunto, portanto, ela trata da procura de padrões e tendencias, sequencias de eventos, analises temporais, etc. 
Isso não quer dizer que a descoberta de dados é algo completamente diferente da exploração dos dados, mas sim, que ela é uma exploração mais especifica para o negocio. Alem disso, a exploração/descoberta de dados também pode ser feita com ferramentas de BI, como power Bi e tableau, elas são muito uteis especialmente na questão de visualização, visto que suas principais funcionalidades são voltadas a criação de dashboards e relatórios.


### Visualização:
[Visualização de dados](https://www.tableau.com/en-gb/learn/articles/data-visualization)

A visualização de dados é referente ao uso de gráficos, dashboards, mapas, etc. para representar as informações retiradas de um conjunto de dados. Ela é especialmente importante por proporcionar uma visão intuitiva e acessível de padrões, tendencias, e outras informações importantes retiradas dos dados. 

No entanto, é importante saber fazer uma boa visualização, ou seja, aquela que ao mesmo tempo que prende a atenção dos clientes ainda consegue expor os dados de maneira acessível e contar uma historia com ele, portanto é recomendável estudar os usos dos principais tipos de gráficos e, principalmente, Storytelling.

#### Visualização interativa de dados:

uma das formas de se transmitir as informações adquiridas de um grande conjunto de dados é através da visualização interativa deles. A forma como as pessoas interagem com os dados influencia como elas os veem e como as decisões serão tomadas, portanto, utilizar ferramentas que permitam uma visualização mais interativa ao invés de estática, pode ajudar na tomada de decisões e no compartilhamento de informações e ideias advindas desses grandes conjuntos de dados. Algumas ferramentas ou bibliotecas que podem ser utilizadas são: PowerBI, Tableu, Dash, plotly, entre outras.
## Metodologia da analise de dados

### Ciclo de análise dos dados
Como a analise muda de negócio para negócio, a forma como uma empresa ou setor trata os dados será a base do método pelo qual eu vou trata-los também, mas existem alguns padrões que podem ser seguidos e adaptados. O principal é o *Ciclo de análise de dados*(Que é algo como o CRISP-DM), esse ciclo visa o entendimento do negocio, modelamento e transformação dos dados. 

O ciclo de análise de dados tem 6 pontos principais:

* 1 - Definição do problema e os objetivos com a análise
	Aqui é verificado qual o problema que a empresa quer esclarecimento e qual será o objetivo final da analise de dados
* 2 - A coleta de dados de diversas fontes
	Aqui é feita a coleta dos dados de diversas fontes, como de planilhas, bancos de dados, web, entre outros
* 3 - A limpeza e preparação dos dados
	Aqui é feita a limpeza e padronização dos dados, para que não haja discrepâncias e erros durante a analise
* 4 - As analises dos dados com estatísticas ou modelos de machine learning
	Aqui é feita a analise em si, ou seja, são visualizados os padrões e tendencias, utilizando predições e aprendizado de máquina em alguns casos.
* 5 - A interpretação e visualização dos dados
	Aqui é feita a visualização dos dados em gráficos e dashboards, organizando eles de forma intuitiva
* 6 - A comunicação e tomada de decisões
	Aqui é feita a apresentação dos resultados da análise para a empresa, e com isso, auxiliando nas tomadas de decisões. Nesta parte considero importante o storytelling, ele será montado na interpretação e visualização, mas aqui é que ele será passado e tratado por gestores ou outros lideres.

### CRISP-DM(Cross Industry Standard Process for Data Mining)
[CRISP DM - Original Doc](https://www.kde.cs.uni-kassel.de/wp-content/uploads/lehre/ws2012-13/kdd/files/CRISPWP-0800.pdf)


### KDD(Knowledge Discovery in Database)

### OSEMN(Obtain, Scrub, Explore, Model, Interpret)
