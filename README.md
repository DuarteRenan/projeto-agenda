# Projeto Agenda de Contatos

Este é um projeto de uma agenda de contatos online, desenvolvido como parte do curso de JavaScript e TypeScript do básico ao avançado. A aplicação permite que usuários se cadastrem, façam login e gerenciem sua própria lista de contatos.

## ✨ Funcionalidades

- **Autenticação de Usuários:** Sistema completo de cadastro e login.
- **Gerenciamento de Contatos (CRUD):**
  - Criar novos contatos com nome, sobrenome, e-mail e telefone.
  - Listar todos os contatos cadastrados pelo usuário.
  - Editar as informações de um contato existente.
  - Excluir um contato.
- **Segurança:** Uso de CSRF tokens para proteção contra ataques e senhas hasheadas.
- **Validação de Dados:** Validação robusta dos dados de entrada tanto no frontend quanto no backend.

## 🚀 Tecnologias Utilizadas

Este projeto foi construído com as seguintes tecnologias:

- **Backend:**
  - [Node.js](https://nodejs.org/en/)
  - [Express.js](https://expressjs.com/pt-br/) para o servidor e gerenciamento de rotas.
  - [MongoDB](https://www.mongodb.com/) como banco de dados NoSQL.
  - [Mongoose](https://mongoosejs.com/) para modelagem dos dados.
  - [EJS (Embedded JavaScript)](https://ejs.co/) como template engine para renderização das views.
  - [dotenv](https://www.npmjs.com/package/dotenv) para gerenciamento de variáveis de ambiente.
  - [validator.js](https://www.npmjs.com/package/validator) para validação de strings.
  - `express-session` e `connect-mongo` para gerenciamento de sessões.
  - `bcryptjs` para hashing de senhas.
  - `csurf` para proteção contra CSRF.

- **Frontend:**
  - HTML5 e CSS3 com Bootstrap.
  - JavaScript para interatividade no lado do cliente.

- **Build Tool:**
  - Webpack para empacotamento dos assets do frontend.

- **Deploy:**
  - A aplicação está hospedada na plataforma Railway.

## ⚙️ Como Executar o Projeto Localmente

Siga os passos abaixo para rodar o projeto em sua máquina.

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/seu-usuario/seu-repositorio.git
    ```

2.  **Instale as dependências:**
    ```bash
    npm install
    ```

3.  **Configure as variáveis de ambiente:**
    Crie um arquivo `.env` na raiz do projeto e adicione as seguintes variáveis, substituindo pelos seus valores:
    ```env
    CONNECTIONSTRING=mongodb+srv://<user>:<password>@<cluster-url>/<database-name>?retryWrites=true&w=majority
    PORT=3000
    SESSION_SECRET=umasecretmuitosegura
    ```

4.  **Inicie o servidor:**
    ```bash
    npm start
    ```

A aplicação estará disponível em `http://localhost:3000`.