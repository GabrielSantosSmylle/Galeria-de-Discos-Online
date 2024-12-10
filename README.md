Projeto de Consumo da API UCS Discos
Este projeto implementa um sistema web para consumir a API UCS Discos API. O objetivo principal é autenticar e realizar chamadas à API para exibir informações de álbuns musicais, utilizando CSS, Bootstrap, HTML e JavaScript para a interface e a interação do usuário.

Funcionalidades Implementadas
1. Autenticação
A chave de API utilizada para autenticar é: 8175fA5f6098c5301022f475da32a2aa.
A autenticação é realizada pelo método de login da API e retorna um token. Este token é utilizado em todas as chamadas subsequentes para acessar os dados.
2. Exibição de Imagens
Ao carregar a página, 12 registros são exibidos automaticamente.
A exibição é organizada em:
2 colunas para larguras maiores que 768px.
1 coluna para larguras menores que 768px.
Apenas as imagens das capas dos álbuns são mostradas inicialmente.
3. Rolagem Infinita
Conforme o usuário chega ao final da página, 4 novos registros são carregados automaticamente.
Quando os 105 registros são exibidos, a rolagem infinita retorna ao primeiro item da lista, criando um loop contínuo.
4. Modal para Detalhes do Álbum
Ao clicar na capa de um álbum, é exibido um modal Bootstrap com as informações detalhadas do registro.
O modal é populado com dados de uma chamada HTTP específica para o registro selecionado, garantindo precisão nas informações.
5. Carregamento e Feedback
Durante qualquer chamada HTTP ou processamento, um loading spinner é exibido para informar ao usuário que a aplicação está carregando.
O feedback visual melhora a experiência do usuário e reduz a possibilidade de confusão.
Tecnologias Utilizadas
HTML: Estruturação da página.
CSS: Estilização básica.
Bootstrap: Layout responsivo e modal para exibição dos detalhes.
Bootstrap consumido diretamente via CDN conforme as recomendações oficiais.
JavaScript:
Manipulação do DOM.
Integração com a API por meio de chamadas AJAX e Fetch.
Implementação da rolagem infinita.
API UCS Discos:
Dados de álbuns recuperados conforme os métodos e descrições no Swagger.
Estrutura do Código
Autenticação
Chamada inicial ao endpoint de autenticação utilizando a chave da API.
Token armazenado e reutilizado em todas as requisições subsequentes.
Exibição de Álbuns
Método inicial para carregar 12 registros.
Função reutilizável para adicionar 4 novos registros à medida que o usuário alcança o final da página.
Modal com Informações Detalhadas
Cada capa de álbum possui um evento de clique.
O evento faz uma requisição à API para obter os detalhes do registro.
Os dados são exibidos no modal de forma organizada.
Layout Responsivo
O layout é ajustado dinamicamente conforme a largura da tela, utilizando as classes responsivas do Bootstrap.
Requisitos Atendidos
Consumo da API UCS Discos com autenticação e utilização do token.
Exibição inicial de 12 registros.
Rolagem infinita para carregar mais dados (4 por vez).
Modal para exibição de informações detalhadas.
Layout responsivo adaptado para diferentes tamanhos de tela.
Feedback visual para processos em andamento.
Configuração e Execução

Instalar Dependências:
O projeto utiliza o Bootstrap e o JavaScript nativo.
Nenhuma dependência adicional precisa ser instalada.

Chave de API:
Certifique-se de que a chave fornecida está configurada corretamente no código.

Executar o Projeto:
Abra o arquivo index.html em qualquer navegador moderno.
Considerações Finais

O sistema foi projetado para ser eficiente e intuitivo. A autenticação foi otimizada para evitar múltiplas chamadas desnecessárias, e a implementação da rolagem infinita garante que os usuários tenham uma experiência contínua. O uso do Bootstrap proporciona uma interface limpa e responsiva. Todas as chamadas HTTP incluem tratamento de erros para lidar com eventuais falhas de rede ou problemas na API.
