# Brain Agriculture

Brain Agriculture é uma aplicação web para o gerenciamento e cadastro de produtores rurais. O projeto é dividido em duas partes principais: um backend (API) e um frontend (React), com integração de banco de dados PostgreSQL. A API está documentada com Swagger para facilitar a visualização e teste dos endpoints.

## Sumário

- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Configuração do Backend](#configuração-do-backend)
- [Configuração do Frontend](#configuração-do-frontend)
- [Rodando a Aplicação com Docker](#rodando-a-aplicação-com-docker)
- [Swagger](#swagger)
- [Como Contribuir](#como-contribuir)

## Tecnologias Utilizadas

### Backend:
- **Node.js** com **NestJS** como framework principal
- **PostgreSQL** como banco de dados
- **TypeORM** para ORM (Mapeamento Objeto-Relacional)
- **Swagger** para documentação da API
- **Docker** para containerização

### Frontend:
- **React** como biblioteca de construção da interface
- **Vite** como bundler para desenvolvimento rápido
- **Nginx** para servir a aplicação em produção
- **Docker** para containerização

---

## Configuração do Backend

### Requisitos
- **Node.js** (versão 20+)
- **PostgreSQL** (versão 13+)

### Passos para rodar o backend localmente

1. **Instalar dependências:**

   No diretório `brain_agriculture`, execute:

   ```bash
   npm install
