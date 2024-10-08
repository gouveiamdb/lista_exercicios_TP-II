## Substituição de Cores em DataFrame de Frutas
Você é responsável pela gestão de uma frutaria que vende maçãs, bananas e uvas. A frutaria tem uma parceria com uma empresa de decoração de eventos que deseja encomendar algumas frutas para uma festa temática. A empresa de decoração solicitou especificamente que as bananas fossem douradas e que as maçãs tivessem uma tonalidade rosa. Porém, o seu sistema de registro das frutas só possui as cores tradicionais: vermelha para maçãs, amarela para bananas e roxa para uvas.

Você precisa de uma solução para atualizar o registro das cores das frutas da frutaria de forma que o pedido da empresa de decoração possa ser atendido.

Crei uma função "substitui_cores" que recebe como parâmetros o DataFrame com as informações das frutas, a coluna das cores que precisa ser atualizada, os valores antigos das cores (vermelha e amarela) e os novos valores que precisam ser substituídos (rosa e dourado). Com essa função, você poderá atender ao pedido da empresa de decoração sem precisar alterar manualmente todas as informações no sistema.

Assinatura da função: substitui_cores(df: pd.DataFrame, coluna: str, dicionario_cores: dict) -> pd.DataFrame. Onde:

df é um DataFrame contendo a coluna a ser modificada;
coluna é uma string representando o nome da coluna a ser modificada;
dicionario_cores é um dicionário onde as chaves representam as cores a serem substituídas e os valores representam as novas cores;
O retorno é um novo DataFrame com as substituições realizadas.
Exemplo:

df = pd.DataFrame({'A': ['maçã', 'banana', 'uva'], 'B': ['vermelha', 'amarela', 'roxa']})
mapeamento_cores = {'vermelha': 'rosa', 'amarela': 'dourada'}

substitui_cores(df, 'B', mapeamento_cores)

>>> 
       A         B
0   maçã      rosa
1  banana   dourada
2    uva      roxa