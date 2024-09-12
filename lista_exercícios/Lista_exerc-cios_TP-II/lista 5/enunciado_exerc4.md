Detecção de Valores Atípicos com Desvio Padrão
Suponha que você trabalhe em uma empresa de manutenção preditiva industrial, responsável por monitorar a saúde de equipamentos críticos por meio de dados de sensores. Para identificar possíveis falhas antes que ocorram, os dados coletados passam por um processo de análise e tratamento.

Escreva uma função em Python que receba um DataFrame contendo dados de temperatura dos sensores instalados nos equipamentos e utilize a técnica do desvio padrão para identificar valores atípicos nessa coluna (Detecção de outlier). A função deve retornar uma lista contendo os registros que contêm valores atípicos na coluna "Temperatura". Esses valores podem indicar possíveis problemas no equipamento e precisam ser investigados pela equipe de manutenção antes que uma falha ocorra e interrompa a produção.

Detecção de outlier é uma técnica utilizada em análise de dados para identificar valores que se distanciam significativamente da maioria dos outros valores em um conjunto de dados. Esses valores, também conhecidos como valores atípicos, podem afetar negativamente a análise estatística e, portanto, precisam ser identificados e tratados adequadamente. Uma das técnicas para detectar outliers é o uso do desvio padrão. O desvio padrão é uma medida de dispersão que indica o quão distante os valores estão da média do conjunto de dados. O desvio padrão é uma medida de dispersão que indica o quanto os dados estão afastados da média. É calculado pela raiz quadrada da variância 
𝜎
2
σ 
2
  e é representado pelo símbolo 
𝜎
σ. Matematicamente, o desvio padrão é dado por:

Alt \sigma = \sqrt{\frac{1}{N}\sum_{i=1}^{N}(x_i-\mu)^2}

Onde N é o número de elementos no conjunto de dados, xi é o valor de cada elemento, 
𝜇
μ é a média dos elementos e 
𝜎
σ é o desvio padrão.

Valores que estão a mais de 3 desvios padrão da média são considerados outliers.

Assinatura da função: identifica_outliers(df: pd.DataFrame, coluna: str) -> pd.DataFrame. A função identifica_outliers recebe dois parâmetros: um DataFrame df contendo os dados a serem analisados e uma string coluna indicando a coluna que deve ser considerada na detecção de outliers. A função retorna um novo DataFrame contendo apenas os registros que contêm valores atípicos na coluna especificada.

Exemplo:

dados = {
     'Temperatura': [30, 32, 35, 28, 27, 31, 400, 29, 33, 34, 36],
     'Pressao': [100, 101, 102, 99, 98, 97, 1003, 100, 101, 99, 102],
     'Umidade': [600, 58, 62, 61, 63, 65, 59, 60, 64, 63, 61]
}

df = pd.DataFrame(dados)

identifica_outliers(df, 'Temperatura')

>>> 
   Temperatura  Pressao  Umidade
6          400     1003       59