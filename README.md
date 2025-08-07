# 🚗 Minimal API - Cadastro de Veículos

Uma API moderna e enxuta para gerenciamento de veículos, construída com .NET 7 e arquitetura orientada por boas práticas de bootcamp.

## 📌 Sobre o Projeto

Este projeto foi desenvolvido como parte de um bootcamp, seguindo o modelo **boilerplate** recomendado por especialistas. Utiliza a abordagem de **Minimal API** do ASP.NET Core para entregar uma solução leve, performática e escalável.

A API permite o **cadastro e gerenciamento de veículos**, com autenticação de administradores via login e senha. Toda a estrutura foi pensada para facilitar a manutenção e evolução do sistema.

## 🧱 Arquitetura e Tecnologias

- **.NET 7** — versão instalada localmente para compatibilidade com os pacotes utilizados
- **ASP.NET Core Minimal API** — estrutura simplificada e direta
- **Entity Framework Core** — mapeamento objeto-relacional com suporte ao MySQL
- **MySQL** — banco de dados relacional para persistência
- **JWT (JSON Web Tokens)** — autenticação segura via token
- **Swagger / OpenAPI** — documentação interativa da API
- **Validação de dados** — login e senha de administradores validados
- **Testes de persistência e requisições** — garantindo integridade e funcionalidade

## 🔐 Autenticação

A API utiliza **JWT** para autenticação de administradores. Após o login, um token é gerado e deve ser enviado nas requisições protegidas.

```http
POST /login
{
  "username": "root",

  "password": "****"
}



