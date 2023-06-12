Para começar com o projeto, verifique se você tem o Node.js na versão 16.17.x ou superior e o npm na versão 8.15.x ou superior instalados. Após clonar o projeto, navegue até o diretório do projeto e execute o seguinte comando para instalar as dependências:

```sh
npm install
```

Em seguida, você precisa especificar a conexão com o banco de dados PostgreSQL criando um arquivo `.env`. Uma vez que o arquivo `.env` seja criado, você pode executar o comando de migração do Prisma para criar as tabelas necessárias com dados iniciais:

```sh
npm run prisma:migrate:deploy
```

Depois disso, você pode popular o banco de dados usando o seguinte comando:

```sh
npx prisma db seed
```

Finalmente, você pode iniciar o servidor de desenvolvimento executando o seguinte comando:

```sh
npm run dev
```

A aplicação estará acessível em [http://localhost:8888](http://localhost:8888) no seu navegador. Por padrão, as credenciais para fazer login são:

- Nome de usuário: user0
- Senha: password
