## Concatenação de Arrays Numpy para Análise de Vendas em Diferentes Regiões
Você é um analista de dados em uma empresa de vendas online e recebeu uma tarefa para analisar as vendas de um determinado produto em diferentes regiões do país. As informações de vendas são armazenadas em dois arrays numpy, um com as vendas da região Sul e outro com as vendas da região Norte. O numpy é uma biblioteca do Python utilizada para trabalhar com matrizes e arrays multidimensionais de forma eficiente, que oferece diversas funções e operações para facilitar a manipulação desses objetos. Uma das vantagens do numpy em relação às listas do Python é a velocidade e eficiência nas operações com arrays. Você precisa concatenar os dois arrays para ter uma visão geral das vendas do produto em todo o país. Para isso, você vai criar uma função chamada concatena_array, que recebe como argumentos dois arrays do tipo numpy e retorna um único array do tipo numpy concatenando os dois.

Exemplo:


vendas_sul = np.array([100, 150, 200])
vendas_norte = np.array([50, 75, 100])

concatena_array(vendas_sul, vendas_norte)

>>> array([100, 150, 200,  50,  75, 100])