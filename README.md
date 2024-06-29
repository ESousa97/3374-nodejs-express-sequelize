<div align="center">

# Projeto Node.js com Express e Sequelize

Este é um projeto *backend* usando **Node.js**, **Express**, e **Sequelize** para gerenciamento de um banco de dados **SQLite**. Estruturado de maneira modular, é ideal para expansão, manutenções eficientes e simples.

</div>

### 🎯 Objetivo

Criar uma aplicação backend robusta com autenticação, operações **CRUD** e interações de banco de dados bem estruturadas.

###  🚀 Início Rápido

Clone o projeto e instale as dependências:

```bash

git clone [URL_DO_REPOSITORIO]
cd [NOME_DO_DIRETORIO]
npm install

```
### ⚙ Configuração do Banco de Dados

Antes de executar o aplicativo, configure o Sequelize:

```bash

npm install -g sequelize-cli
sequelize db:migrate
sequelize db:seed:all

```

### 🌐 Execução

Para iniciar o servidor local:

```bash

npm run dev

```
O servidor estará rodando em http://localhost:3000.

### 📂 Estrutura do Projeto

| Componente             | Descrição                                                                         |
|------------------------|-----------------------------------------------------------------------------------|
| `🔹 src/app.js`         | Arquivo principal do Express que **inicializa o servidor**.                        |
| `🔹 src/config`         | Contém as **configurações globais** e de banco de dados.                          |
| `🔹 src/controllers`    | **Controladores** que processam as requisições da API.                            |
| `🔹 src/migrations`     | **Migrações do Sequelize** para gestão da estrutura do banco.                      |
| `🔹 src/models`         | **Modelos do Sequelize** que mapeiam para as tabelas do banco.                     |
| `🔹 src/routes`         | **Rotas** que definem os endpoints da API e suas ações.                            |
| `🔹 src/seeders`        | **Seeders** para preencher o banco de dados com dados iniciais.                    |
| `🔹 src/services`       | **Serviços** que contêm lógica de negócios e interações com banco.                 |

### 💬 FAQ

#### Como resolver conflitos de dependência?

Assegure-se de usar a versão correta do Node.js. Remova `node_modules` e `package-lock.json` e execute `npm install` novamente.

#### Migrações não estão sendo aplicadas?

Certifique-se que as configurações no `config.json` estão corretas e que o banco de dados está acessível.

#