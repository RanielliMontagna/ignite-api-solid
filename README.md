<h1 align="center">Ignite - Api Solid</h1>

<p align="center">
  <img
    alt="GitHub top language"
    src="https://img.shields.io/github/languages/top/raniellimontagna/ignite-api-solid?f&style=flat-square"
  />
  <img
    alt="GitHub language count"
    src="https://img.shields.io/github/languages/count/raniellimontagna/ignite-api-solid?f&style=flat-square"
  />
</p>

## 📖 Sobre

### ✨ API

O Projeto Ignite - Api Solid é uma aplicação que foi desenvolvida durante o curso Ignite da Rocketseat.
O objetivo do projeto é colocar em prática os conceitos de SOLID, TDD e Clean Architecture.

### 🏋️ Sistema

O sistema é em um estilo GymPass, com o intuito de realizar check-ins em academias.
Para isso, as seguintes premissas foram levadas em consideração:

#### RFs (Requisitos Funcionais)

- [x] Deve ser possível se cadastrar;
- [x] Deve ser possível se autenticar;
- [x] Deve ser possível obter o perfil de um usuário logado;
- [x] Deve ser possível obter o número de check-ins realizados pelo usuário logado;
- [x] Deve ser possível o usuário obter seu histórico de check-ins;
- [x] Deve ser possível o usuário buscar academias próximas;
- [x] Deve ser possível o usuário buscar academias pelo nome;
- [x] Deve ser possível o usuário realizar check-in em uma academia;
- [x] Deve ser possível validar o check-in de um usuário;
- [x] Deve ser possível cadastrar uma academia;

#### RNs (Regras de Negócio)

- [x] O usuário não deve poder se cadastrar com um e-mail duplicado;
- [x] O usuário não pode fazer 2 check-ins no mesmo dia;
- [x] O usuário não pode fazer check-in se não estiver perto (100m) da academia;
- [x] O check-in só pode ser validado até 20 minutos após ser criado;
- [x] O check-in só pode ser validado por administradores;
- [x] A academia só pode ser cadastrada por administradores;

#### RNFs (Requisitos Não Funcionais)

- [x] A senha do usuário precisa estar criptografada;
- [x] Os dados da aplicação precisam estar persistidos em um banco PostgreSQL;
- [x] Todas listas de dados precisam estar paginadas com 20 itens por página;
- [x] O usuário deve ser identificado por um JWT (JSON Web Token);

## 🛣️ Rotas

| Método  | Rota                     | Descrição                        |
| ------- | ------------------------ | -------------------------------- |
| `POST`  | `/users`                 | Cria um usuário                  |
| `POST`  | `/sessions`              | Autentica um usuário             |
| `GET`   | `/me`                    | Obtém o perfil do usuário logado |
| `PATCH` | `/token/refresh`         | Atualiza o token do usuário      |
| ------- | ----------------         | -------------------------------- |
| `POST`  | `/gyms`                  | Cria uma academia                |
| `GET`   | `/gyms/search`           | Busca academias por nome         |
| `GET`   | `/gyms/nearby`           | Busca academias próximas         |
| ------- | ----------------         | -------------------------------- |
| `GET`   | `/check-ins/history`     | Obtém o histórico de check-ins   |
| `GET`   | `/check-ins/metrics`     | Obtém o número de check-ins      |
| `POST`  | `/gyms/:gymId/check-ins` | Realiza um check-in              |
| `PATCH` | `/check-ins/:checkInId`  | Valida um check-in               |

## 🚀 Tecnologias

- [Node.js](https://nodejs.org/en/) - Interpretador de JavaScript para construção do servidor;
- [Fastify](https://www.fastify.io/) - Framework para construção de APIs;
- [TypeScript](https://www.typescriptlang.org/) - Superset JavaScript;
- [Prisma](https://www.prisma.io/) - ORM para banco de dados;
- [PostgreSQL](https://www.postgresql.org/) - Banco de dados relacional;
- [Docker](https://www.docker.com/) - Container para banco de dados;
- [Vitest](https://vitest.dev/) - Test Runner para TypeScript;
- [Supertest](https://www.npmjs.com/package/supertest) - Biblioteca para testes de integração;
- [BCrypt](https://www.npmjs.com/package/bcrypt) - Biblioteca para criptografia de senhas;
- [Zod](https://www.npmjs.com/package/zod) - Biblioteca para validação de dados;

## 📦 Instalação

```bash
# Clone o repositório
$ git clone

# Acesse a pasta do projeto
$ cd ignite-api-solid

# Instale as dependências
$ npm install

# Execute a aplicação
$ npm run dev

# A aplicação será aberta na porta:3333 - acesse http://localhost:3333
```

## 🧪 Testes

### ❇️ Testes Unitários

```bash
# Execute os testes unitários
$ npm run test

# Execute os testes unitários com coverage
$ npm run test:coverage
```

### ❇️ Testes de Integração

```bash
# Execute os testes de integração
$ npm run test:e2e
```

### 🖊️ Autor - [@raniellimontagna](https://www.github.com/raniellimontagna)
