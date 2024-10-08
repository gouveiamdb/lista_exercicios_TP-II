## Substituição Condicional de Valores em um DataFrame
Imagine que você é um cientista de dados responsável pela análise de dados de uma empresa que produz chocolates. Você recebeu um DataFrame que contém informações sobre o processo produtivo, incluindo a temperatura, o tempo de mistura e a qualidade dos ingredientes.

Durante a análise, você percebeu que alguns registros apresentam um valor muito alto na coluna que representa a qualidade dos ingredientes, o que pode afetar a qualidade final do produto. Para resolver esse problema, você decidiu criar uma função que substitua todos os valores iguais ou maiores que um determinado limite por um valor pré-determinado, para garantir que a qualidade dos ingredientes esteja sempre dentro dos padrões de qualidade estabelecidos pela empresa.

Assim, você cria uma função que recebe o DataFrame com os dados dos ingredientes, a coluna, o valor limite que deve ser verificado e o valor que deve ser substituído caso o valor seja maior ou igual ao limite. Essa função irá te ajudar a garantir que a qualidade dos ingredientes utilizados na produção dos chocolates seja sempre a melhor possível, resultando em um produto final de qualidade superior e satisfação dos clientes.

Assinatura da função: substitui_valores(df: pd.DataFrame, coluna:str, limite: int, valor_padrao: int) -> pd.DataFrame. A função substitui_valores recebe como parâmetros um DataFrame df, uma string coluna indicando a coluna a ser modificada, um valor limite que determina o limite a partir do qual os valores serão substituídos e um valor valor_padrao que será o valor utilizado para substituição. A função retorna um DataFrame com os valores da coluna especificada modificados, substituindo os valores maiores ou iguais a limite pelo valor valor padrão.

Exemplo:

df = pd.DataFrame({'A': [1, 2, 3], 'B': [4, 5, 6]})

substitui_valores(df, 'B', 5, 10)