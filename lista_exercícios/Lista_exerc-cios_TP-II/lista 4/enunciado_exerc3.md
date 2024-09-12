## Cálculo do Índice de Massa Corporal (IMC) em um Dataframe
Você é um nutricionista e precisa criar uma ferramenta para calcular o Índice de Massa Corporal (IMC) de seus pacientes. Para isso, você pode utilizar a biblioteca Pandas do Python. Ela é uma biblioteca Python de código aberto que fornece ferramentas de análise e manipulação de dados de forma rápida e eficiente. O Pandas permite trabalhar com dados em formato de tabela, chamados de DataFrames, com colunas de tipos diferentes, além de oferecer funcionalidades para indexação, agregação, seleção, filtragem e visualização dos dados. Com essa biblioteca, é possível realizar tarefas de limpeza, transformação e modelagem de dados, sendo uma ferramenta muito útil em áreas como ciência de dados, finanças, economia, entre outras.

Escreva uma função chamada calcula_imc que receba um DataFrame pandas contendo as informações de nome, idade, sexo, altura e peso de um paciente, calcule o IMC e adicione uma nova coluna no DataFrame contendo o resultado do cálculo. Em seguida, a função deve retornar o DataFrame modificado.

A fórmula para calcular o IMC:

Alt IMC = \frac{peso}{altura^{2}}

Assinatura da função: calcula_imc(df: pd.DataFrame) -> pd.DataFrame

Exemplo:

dados = {
    "Nome": ["João", "Maria", "José", "Ana", "Carlos"],
    "Idade": [30, 25, 40, 35, 28],
    "Sexo": ["M", "F", "M", "F", "M"],
    "Altura": [1.75, 1.68, 1.80, 1.65, 1.72],
    "Peso": [70, 55, 85, 75, 80]
}
df = pd.DataFrame(dados)

calcula_imc(df)

>>> 
     Nome  Idade Sexo  Altura  Peso        IMC
0    João     30    M    1.75    70  22.857143
1   Maria     25    F    1.68    55  19.486961
2    José     40    M    1.80    85  26.234568
3     Ana     35    F    1.65    75  27.548209
4  Carlos     28    M    1.72    80  27.041644