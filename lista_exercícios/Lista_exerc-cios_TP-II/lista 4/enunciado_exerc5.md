## Cálculo da soma dos elementos de cada coluna em uma matriz usando NumPy
O processamento digital de imagens é uma área que utiliza técnicas computacionais para processar e analisar imagens digitais. Uma das bibliotecas utilizadas nessa área é o NumPy, uma biblioteca Python que permite trabalhar com matrizes multidimensionais e oferece diversas funções e operações matemáticas.

Suponha que você seja um desenvolvedor de software de processamento digital de imagens e foi designado para criar uma função que calcule a soma dos elementos de cada coluna de uma matriz de entrada. A matriz de entrada pode ter qualquer tamanho e é armazenada como um array NumPy.

Assinatura da função: soma_colunas(matriz: np.ndarray) -> np.ndarray

Exemplo:


matriz = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])

soma = soma_colunas(matriz)

>>> array([12, 15, 18])