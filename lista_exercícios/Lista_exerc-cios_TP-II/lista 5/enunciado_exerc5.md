Exclusão de Registros em DataFrame
Suponha que você trabalhe em uma empresa que coleta e armazena informações de clientes em um DataFrame para fins de análise de mercado. Devido à entrada em vigor da Lei Geral de Proteção de Dados (LGPD), é necessário excluir os registros de clientes que solicitaram a exclusão de seus dados pessoais.

A LGPD é a Lei Geral de Proteção de Dados, que entrou em vigor em setembro de 2020 e tem como objetivo regulamentar o uso, a proteção e a transferência de dados pessoais no Brasil. A lei estabelece regras para empresas e órgãos públicos em relação à coleta, tratamento, armazenamento e compartilhamento de informações de indivíduos, garantindo a privacidade e a segurança dos dados. A LGPD também prevê sanções para quem descumpri-la, como multas e até mesmo a proibição do tratamento de dados pessoais.

Escreva uma função que receba um DataFrame com informações de clientes e uma lista de índices a serem excluídos. A função deve remover os registros correspondentes aos índices da lista e retornar o DataFrame modificado.

O objetivo dessa função é garantir a conformidade com as regulamentações da LGPD e garantir a privacidade dos dados pessoais dos clientes.

Assinatura da função: deleta_registros(df: pd.DataFrame, indices: list) -> pd.DataFrame. Essa função recebe um DataFrame df e uma lista de índices indices que indicam quais registros devem ser removidos do DataFrame. Em seguida, a função retorna um novo DataFrame que é uma cópia do DataFrame original com os registros indicados pelos índices removidos.

Exemplo:

df = pd.DataFrame({'Nome': ['João', 'Maria', 'Pedro', 'Ana'], 
                   'Idade': [25, 30, 40, 20], 
                   'Cidade': ['São Paulo', 'Rio de Janeiro', 'Belo Horizonte', 'Porto Alegre']})

deleta_registros(df, [1, 3])

>>> 
    Nome  Idade         Cidade
0   João     25      São Paulo
2  Pedro     40  Belo Horizonte