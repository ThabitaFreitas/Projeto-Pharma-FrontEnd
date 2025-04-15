# ⋆˚✿˖° FrontEnd- Sistema de Gestão de Ações de Marketing ⋆˚✿˖°

Este repositório contém o frontend para gestão de verbas de ações de marketing. Ele se conecta ao backend Flask que permite realizar operações CRUD em ações de marketing.

## Tecnologias Utilizadas

- **HTML5** - Linguagem de marcação usada para estruturar o conteúdo da página.
- **CSS** - Estilos para a formatação da interface.
- **JavaScript** (jQuery) - Manipulação de dados e interação com a API.
- **Bootstrap 5** - Framework CSS para um layout responsivo e componentes prontos.
- **DataTables** - Biblioteca para melhorar a apresentação de tabelas dinâmicas.
- **jQuery Mask Plugin** - Para mascarar entradas de data.

---

## 📁 Estrutura do Projeto 

A estrutura do projeto frontend é simples e organizada:  

**📄 index.html**  
Arquivo HTML principal  

**🎨 style.css**  
Arquivo de estilo personalizado  

**🖼️ pharmaviews.png**  
Logotipo da empresa  

**📄 README.md**  
Documentação do projeto  


---

## Como Rodar o Frontend

### Pré-requisitos

Não há necessidade de instalar pacotes específicos para rodar o frontend, pois ele utiliza links CDN para as bibliotecas necessárias. Porém, se você deseja rodar o projeto localmente, siga as instruções abaixo.

### Rodando o Frontend

1. Clone o repositório:
   ```bash
   git clone https://github.com/SEU-REPOSITORIO/frontend.git
   cd frontend
# 📌 Guia de Uso do Frontend - Gestão de Ações de Marketing  

## 🚀 Abrindo o Projeto  
1. Localize o arquivo `index.html`.  
2. Abra-o no seu navegador preferido.  

---  

## 🎯 Funcionalidades  
O frontend permite gerenciar ações de marketing com as seguintes opções:  

✅ **Adicionar Nova Ação**  
- Escolha o tipo de ação.  
- Insira a data prevista.  
- Defina o valor do investimento.  

✅ **Visualizar Ações Cadastradas**  
- Tabela dinâmica exibindo todas as ações de marketing.  

✅ **Editar Ações**  
- Modifique os dados de uma ação já cadastrada.  

✅ **Excluir Ações**  
- Remova uma ação da tabela.  

---  

## 🔗 Comunicação com a API  
A aplicação realiza requisições HTTP para interagir com o backend:  

🔹 `POST` → Criar novas ações.  
🔹 `PATCH` → Editar ações existentes.  
🔹 `DELETE` → Excluir ações.  
🔹 `GET` → Listar todas as ações de marketing.  

---  

## 📊 Estrutura da Tabela  
A tabela de ações de marketing contém as seguintes colunas:  

📌 **Ação** → Tipo da ação (Ex.: Palestra, Evento, Apoio Gráfico).  
📅 **Data Prevista** → Quando a ação está programada.  
💰 **Investimento Previsto** → Valor estimado do investimento.  
🛠 **Ações** → Botões de **Editar** e **Excluir** para cada linha.  

---  

## ✅ Validações no Frontend  
Antes de enviar os dados para a API, algumas regras são verificadas:  

✔ **Ação:** O usuário deve selecionar um tipo de ação válido (*Palestra, Evento, Apoio Gráfico*).  
✔ **Data:** Formato obrigatório `DD/MM/AAAA` e e deve estar pelo menos **10 dias no futuro**.  
✔ **Investimento:** O valor precisa ser **numérico e positivo**.  

---  

## 📦 Dependências  
O projeto utiliza as seguintes bibliotecas:  

📌 **Bootstrap** → Estilização responsiva e rápida.  
📌 **jQuery** → Manipulação de DOM e requisições AJAX.  
📌 **DataTables** → Tabelas dinâmicas com pesquisa, ordenação e paginação.  
📌 **jQuery Mask Plugin** → Máscara para formatação de datas
