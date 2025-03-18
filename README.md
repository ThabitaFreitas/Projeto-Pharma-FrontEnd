# Projeto Pharma - Frontend

Este repositório contém o frontend para gestão de verbas de ações de marketing. Ele se conecta ao backend Flask que permite realizar operações CRUD em ações de marketing.

## Tecnologias Utilizadas

- **HTML5** - Linguagem de marcação usada para estruturar o conteúdo da página.
- **CSS** - Estilos para a formatação da interface.
- **JavaScript** (jQuery) - Manipulação de dados e interação com a API.
- **Bootstrap 5** - Framework CSS para um layout responsivo e componentes prontos.
- **DataTables** - Biblioteca para melhorar a apresentação de tabelas dinâmicas.
- **jQuery Mask Plugin** - Para mascarar entradas de data.

---

## Estrutura do Projeto

A estrutura do projeto frontend é simples e organizada:

/frontend │ ├── index.html # Arquivo HTML principal ├── style.css # Arquivo de estilo personalizado ├── pharmaviews.png # Logotipo da empresa ├── /node_modules # Diretório de dependências do Node (se for utilizado) └── README.md # Este arquivo

yaml
Copy

---

## Como Rodar o Frontend

### Pré-requisitos

Não há necessidade de instalar pacotes específicos para rodar o frontend, pois ele utiliza links CDN para as bibliotecas necessárias. Porém, se você deseja rodar o projeto localmente, siga as instruções abaixo.

### Rodando o Frontend

1. Clone o repositório:
   ```bash
   git clone https://github.com/SEU-REPOSITORIO/frontend.git
   cd frontend
Abra o arquivo index.html em seu navegador preferido.
Funcionalidades
O frontend permite ao usuário gerenciar as ações de marketing, com a possibilidade de:

Adicionar nova ação: Escolher o tipo de ação, inserir a data prevista e o valor do investimento.
Visualizar ações cadastradas: Tabelas dinâmicas que mostram as ações de marketing.
Editar ações: Alterar os dados de uma ação já cadastrada.
Excluir ações: Remover uma ação da tabela.
Interação com a API
A aplicação se comunica com a API backend através de requisições HTTP:

POST: Criação de novas ações.
PATCH: Edição de ações existentes.
DELETE: Exclusão de ações.
GET: Listagem de todas as ações de marketing.
Estrutura da Tabela
A tabela de ações de marketing contém as seguintes colunas:

Ação: Tipo da ação (Ex.: Palestra, Evento, Apoio Gráfico).
Data Prevista: A data em que a ação está prevista para acontecer.
Investimento Previsto: O valor estimado para o investimento na ação.
Além disso, existem botões de Editar e Excluir para cada linha, permitindo que o usuário altere ou remova uma ação de marketing.

Validations
As validações são feitas diretamente no frontend antes de enviar os dados para a API:

Ação: O usuário deve selecionar um tipo de ação válido (Palestra, Evento, Apoio Gráfico).
Data: O formato da data deve ser DD/MM/AAAA e a data precisa ser no futuro (pelo menos 10 dias após a data atual).
Investimento: O campo de investimento deve ser um valor numérico positivo.
Dependências
O projeto depende das seguintes bibliotecas:

Bootstrap: Framework para estilização rápida e responsiva.
jQuery: Biblioteca para manipulação de DOM e requisições AJAX.
DataTables: Para criar tabelas dinâmicas com suporte a ordenação, pesquisa e paginação.
jQuery Mask Plugin: Para mascarar o campo de data.
