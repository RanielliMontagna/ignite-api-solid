# Ignite - Api Solid

<p align="center">
  <img src="https://img.shields.io/static/v1?label=Status&message=Em%20Constru%C3%A7%C3%A3o&color=red&style=for-the-badge" />
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
- [ ] Deve ser possível obter o número de check-ins realizados pelo usuário logado;
- [ ] Deve ser possível o usuário obter seu histórico de check-ins;
- [ ] Deve ser possível o usuário buscar academias próximas;
- [ ] Deve ser possível o usuário buscar academias pelo nome;
- [ ] Deve ser possível o usuário realizar check-in em uma academia;
- [ ] Deve ser possível validar o check-in de um usuário;
- [ ] Deve ser possível cadastrar uma academia;

#### RNs (Regras de Negócio)

- [x] O usuário não deve poder se cadastrar com um e-mail duplicado;
- [ ] O usuário não pode fazer 2 check-ins no mesmo dia;
- [ ] O usuário não pode fazer check-in se não estiver perto (100m) da academia;
- [ ] O check-in só pode ser validado até 20 minutos após ser criado;
- [ ] O check-in só pode ser validado por administradores;
- [ ] A academia só pode ser cadastrada por administradores;

#### RNFs (Requisitos Não Funcionais)

- [x] A senha do usuário precisa estar criptografada;
- [x] Os dados da aplicação precisam estar persistidos em um banco PostgreSQL;
- [ ] Todas listas de dados precisam estar paginadas com 20 itens por página;
- [ ] O usuário deve ser identificado por um JWT (JSON Web Token);

#### 🖊️ Autor - [@raniellimontagna](https://www.github.com/raniellimontagna)
