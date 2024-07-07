<div align="center">

# Projeto Node.js com Express e Sequelize

Este projeto backend utiliza **Node.js**, **Express** e **Sequelize** para gerenciar um banco de dados **SQLite** para desenvolvimento e **MySQL** para produção e testes. Projetado de forma modular, ele é ideal para expansões e manutenções eficientes.

</div>

### 🎯 Objetivo

Desenvolver uma aplicação backend robusta que suporte autenticação, operações CRUD completas e interações complexas de banco de dados, facilitando o gerenciamento de entidades educacionais como categorias, cursos, matrículas e pessoas.

### 🚀 Início Rápido

Clone o repositório e instale as dependências:

```bash
git clone [URL_DO_REPOSITORIO]
cd [NOME_DO_DIRETORIO]
npm install
```

## ⚙ Configuração do Banco de Dados

Configure o Sequelize antes de executar a aplicação:

```bash

npm install -g sequelize-cli
sequelize db:migrate
sequelize db:seed:all

```

## 🌐 Execução

Para iniciar o servidor localmente:

```bash

npm run dev

```

O servidor estará ativo em: http://localhost:3000.

## 📂 Estrutura do Projeto

### 📂 Estrutura do Projeto

| Componente           | Descrição                                                                         |
|----------------------|-----------------------------------------------------------------------------------|
| `🔹src/app.js`       | Arquivo principal do Express que **inicializa o servidor**.                       |
| `🔹src/config`       | Contém as **configurações globais** e de banco de dados para diferentes ambientes.|
| `🔹src/controllers`  | **Controladores** que processam as requisições da API, estendendo um controlador base. |
| `🔹src/migrations`   | **Migrações do Sequelize** para gestão da estrutura do banco.                     |
| `🔹src/models`       | **Modelos do Sequelize** que mapeiam as tabelas do banco e definem relações.      |
| `🔹src/routes`       | **Rotas** que definem os endpoints da API e suas ações, organizadas por entidade. |
| `🔹src/seeders`      | **Seeders** para preencher o banco de dados com dados iniciais.                   |
| `🔹src/services`     | **Serviços** que contêm lógica de negócio e interações com o banco, utilizando uma classe de serviços base para CRUD. |


## 💬 FAQ

### Como resolver conflitos de dependência?

Assegure-se de usar a versão correta do `Node.js`. Remova `node_modules` e `package-lock.json` e execute `npm install` novamente.

### Migrações não estão sendo aplicadas?

Certifique-se de que as configurações no `config/config.json` estão corretas e que o banco de dados está acessível.

##