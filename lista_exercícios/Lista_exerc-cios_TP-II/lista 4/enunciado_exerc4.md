## Criação de DataFrame Pandas para Apoio a Planejamento de Dieta
Suponha que você esteja desenvolvendo um sistema para apoio a planejamento de dieta, que tem como objetivo auxiliar as pessoas a atingirem seus objetivos de saúde por meio de uma alimentação equilibrada. Uma das funcionalidades desse sistema é o registro das informações pessoais dos usuários, tais como nome, idade, sexo, altura e peso.

Para armazenar essas informações, você pode utilizar a biblioteca pandas do Python, que permite trabalhar com tabelas de dados (DataFrames). Pandas é uma biblioteca Python de código aberto que fornece ferramentas de análise e manipulação de dados de forma rápida e eficiente. O Pandas permite trabalhar com dados em formato de tabela, chamados de DataFrames, com colunas de tipos diferentes, além de oferecer funcionalidades para indexação, agregação, seleção, filtragem e visualização dos dados. Com essa biblioteca, é possível realizar tarefas de limpeza, transformação e modelagem de dados, sendo uma ferramenta muito útil em áreas como ciência de dados, finanças, economia, entre outras.

Crie uma função chamada cria_dataframe que receba uma lista contendo as informações de nome, idade, sexo, altura e peso de 
𝑛
n pessoas e retorne um DataFrame com essas informações.

Assinatura da função: cria_dataframe(lista: list) -> pd.DataFrame

Exemplo:

dados = [["Maria", 30, "F", 1.65, 65.0], 
         ["João", 25, "M", 1.75, 80.0], 
         ["Ana", 40, "F", 1.70, 70.0], 
         ["Pedro", 20, "M", 1.80, 75.0], 
         ["Lúcia", 35, "F", 1.60, 55.0]]

cria_dataframe(dados)

>>> 
     Nome  Idade Sexo  Altura  Peso
0   Maria     30    F    1.65  65.0
1    João     25    M    1.75  80.0
2     Ana     40    F    1.70  70.0
3   Pedro     20    M    1.80  75.0
4   Lúcia     35    F    1.60  55.0