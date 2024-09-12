## Cálculo da Imagem Integral de uma Matriz de Pixels Utilizando NumPy em Processamento de Imagens
Você é um cientista de dados de uma empresa de tecnologia que está desenvolvendo um algoritmo de detecção de bordas em imagens digitais. Para implementar o algoritmo, é necessário calcular a imagem integral da imagem original.

Imagem integral é um conceito muito utilizado no processamento de imagens para acelerar o cálculo de operações como filtros, detecção de bordas e reconhecimento de objetos. Ela consiste em uma matriz que armazena a soma acumulada dos pixels de uma imagem em todas as posições à esquerda e acima de um determinado pixel. Dessa forma, o valor de um determinado retângulo na imagem pode ser calculado em tempo constante, independente do tamanho do retângulo. A imagem integral é amplamente utilizada em aplicações de visão computacional, como detecção de faces e análise de objetos em tempo real.

A equação matemática que define a imagem integral é:

Alt \mathrm{I}(x,y) = \sum_{i=0}^{x}\sum_{j=0}^{y} \mathrm{img}(i,j)

Onde I(x,y) é o valor da imagem integral na posição (x,y) e img(x,y) é o valor da imagem original na mesma posição. A imagem integral é usada em processamento de imagens para calcular a soma dos pixels em uma região retangular da imagem de forma eficiente.

Escreva uma função chamada "calcula_imagem_integral" que recebe como entrada uma matriz numpy e retorna outra matriz numpy com a imagem integral correspondente.

Assinatura da função: calcula_imagem_integral(imagem: np.ndarray) -> np.ndarray

Exemplo:


imagem = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
imagem_integral = calcula_imagem_integral(imagem)

>>> array([[1 , 3 , 6 ],
           [5 , 12, 21],
           [12, 27, 45]])