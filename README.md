# 🎵 Projeto de Exibição de Álbuns Musicais com API UCS Discos

## 🌟 Funcionalidades
- **🔑 Autenticação**:
  - Utiliza a chave de API: `8175fA5f6098c5301022f475da32a2aa`.
  - Gera um **token** para chamadas subsequentes.
- **🖼️ Exibição de Capas**:
  - Exibe inicialmente **12 capas de álbuns** ao abrir a página.
  - Layout responsivo:
    - **2 colunas** para larguras maiores que **768px**.
    - **1 coluna** para larguras menores.
- **♾️ Rolagem Infinita**:
  - Carrega **4 novos registros** ao alcançar o final da página.
  - Após os 105 registros, retorna ao início da lista.
- **📋 Detalhes em Modal**:
  - Clique em uma capa para abrir um **modal Bootstrap** com informações detalhadas do álbum.
  - Modal populado com dados de uma requisição específica para o álbum.

## 🛠️ Tecnologias Utilizadas
- **HTML/CSS**: Estrutura e estilo da página.
- **Bootstrap**: Layout responsivo e modal (consumido via CDN).
- **JavaScript**:
  - **AJAX** para autenticação e carregamento de dados.
  - **Fetch** para chamadas específicas.
  - Tratamento de erros e manipulação do DOM.

## ⚙️ Como Funciona
1. **Autenticação**:
   - Realizada automaticamente ao carregar a página para obter o **token**.
2. **Exibição Inicial**:
   - Mostra **12 capas** em um layout responsivo.
3. **Rolagem Infinita**:
   - Adiciona mais álbuns conforme o usuário navega.
4. **Modal com Detalhes**:
   - Exibido ao clicar em uma capa de álbum, mostrando informações detalhadas.

## 🖼️ Visual
- Layout organizado e adaptável para diferentes tamanhos de tela.
- Feedback visual de **loading** enquanto as requisições estão em andamento.

🎯 *Experiência fluida e intuitiva para navegar por álbuns musicais!*
