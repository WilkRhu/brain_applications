Brain Agriculture
Brain Agriculture é uma aplicação web para o gerenciamento e cadastro de produtores rurais. O projeto é dividido em duas partes principais: um backend (API) e um frontend (React), com integração de banco de dados PostgreSQL. A API está documentada com Swagger para facilitar a visualização e teste dos endpoints.

Sumário
Tecnologias Utilizadas
Configuração do Backend
Configuração do Frontend
Rodando a Aplicação com Docker
Swagger
Como Contribuir
Tecnologias Utilizadas
Backend:
Node.js com NestJS como framework principal
PostgreSQL como banco de dados
TypeORM para ORM (Mapeamento Objeto-Relacional)
Swagger para documentação da API
Docker para containerização
Frontend:
React como biblioteca de construção da interface
Vite como bundler para desenvolvimento rápido
Nginx para servir a aplicação em produção
Docker para containerização
Configuração do Backend
Requisitos
Node.js (versão 20+)
PostgreSQL (versão 13+)
Passos para rodar o backend localmente
Instalar dependências:

No diretório brain_agriculture, execute:

bash
Copiar código
npm install
Configurar o banco de dados:

Certifique-se de ter o PostgreSQL rodando e crie um banco de dados com o nome brain_agriculture. Em seguida, configure as credenciais de conexão no arquivo .env dentro do diretório brain_agriculture.

Exemplo de um arquivo .env:

env
Copiar código
POSTGRES_USER=postgres
POSTGRES_PASSWORD=123
POSTGRES_DB=brain_agriculture
POSTGRES_HOST=localhost
POSTGRES_PORT=5432
Rodar migrações:

Execute o seguinte comando para aplicar as migrações do banco de dados:

bash
Copiar código
npm run typeorm migration:run
Rodar a aplicação:

Para rodar a aplicação em modo de desenvolvimento, execute:

bash
Copiar código
npm run start:dev
A aplicação estará disponível em http://localhost:3001.

Swagger
A documentação da API está disponível em:

bash
Copiar código
http://localhost:3001/api
Através da interface do Swagger, você pode testar os endpoints e verificar a documentação completa da API.

Configuração do Frontend
Requisitos
Node.js (versão 20+)
Passos para rodar o frontend localmente
Instalar dependências:

No diretório brain_agriculture_front, execute:

bash
Copiar código
npm install
Rodar a aplicação:

Para iniciar a aplicação em modo de desenvolvimento, execute:

bash
Copiar código
npm run dev
A aplicação estará disponível em http://localhost:3000.

Rodando a Aplicação com Docker
A aplicação está preparada para rodar via Docker, tanto backend quanto frontend, em um ambiente integrado.

Passos para rodar com Docker
Certifique-se de que o Docker e o Docker Compose estão instalados na sua máquina.

No diretório raiz do projeto (onde está o docker-compose.yml), execute:

bash
Copiar código
docker-compose up --build
Isso irá:

Construir e iniciar o backend, frontend e o PostgreSQL.
A aplicação backend estará disponível em http://localhost:3001.
A aplicação frontend estará disponível em http://localhost:3000.
Verificar o Swagger:

O Swagger estará disponível na URL:

bash
Copiar código
http://localhost:3001/api
Swagger
O Swagger é uma ferramenta para documentar a API de forma interativa. Você pode acessar a documentação e testar os endpoints diretamente pelo navegador.

URL do Swagger: http://localhost:3001/api
Endpoints Principais
A API inclui os seguintes recursos principais:

Produtores Rurais: Cadastro, atualização, listagem e remoção de produtores rurais.
