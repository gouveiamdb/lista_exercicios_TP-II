## Criação de uma Matriz Identidade Usando NumPy
No processamento digital de imagens, é comum utilizar matrizes para representar imagens e aplicar operações matemáticas sobre elas. Uma operação comum é a multiplicação de uma matriz por um escalar, que pode ser usado para ajustar o brilho ou a intensidade de cores de uma imagem. O NumPy é uma biblioteca do Python que permite trabalhar com matrizes multidimensionais e oferece diversas funções e operações matemáticas.

Nesse contexto, crie uma função chamada cria_matriz_identidade que receba dois parâmetros: o tamanho da matriz (n) e o fator de multiplicação (m). A função deve retornar uma matriz identidade de tamanho n x n multiplicada pelo fator m, representada como um array numpy.

Assinatura da função: cria_matriz_identidade(n:int, m:float) -> np.ndarray

Exemplo:


cria_matriz_identidade(3, 2)

>>> array([[2., 0., 0.],
           [0., 2., 0.],
           [0., 0., 2.]])