## Criação de Série Pandas a partir de Listas de Valores e Índices
Suponha que você é um analista de dados de uma empresa de varejo e precisa manipular uma lista com informações de vendas de diferentes produtos. Para facilitar a análise desses dados, você decidiu criar uma função que transforma essa lista em uma série do pandas.

Crie uma função que receba uma lista de valores e uma lista de índices e retorne uma série pandas com esses dados.

Assinatura da função: criar_serie(valores: list, indices: list) -> pd.Series. A função criar_serie recebe como entrada duas listas: valores, contendo os valores da série, e indices, contendo os rótulos que serão utilizados como índice da série.

Exemplo:

valores = [100, 200, 150, 300]
indices = ['Produto A', 'Produto B', 'Produto C', 'Produto D']

criar_serie(valores, indices)

>>> 
Produto A    100
Produto B    200
Produto C    150
Produto D    300
dtype: int64