<h1 align="center">
  NLW Heat - Node.js
</h1>

## :rocket: Tecnologias

Foram usadas as seguintes tecnologias:

- [Express](https://expressjs.com/pt-br/)
- [Prisma](https://www.prisma.io/)
- [Typescript](https://www.typescriptlang.org)
- [JSON Web Token](https://jwt.io/)
- [Socket.IO](https://socket.io/)

## :computer: Projeto

Projeto desenvolvido em [Node.js](https://nodejs.org/en/) durante o Next Level Week Heat pela [Rocketseat](https://rocketseat.com.br), para realizar um login com Github e participar de um chat sobre o evento. O grande diferencial dessa edição foi o uso do Prisma, pois é bem simples de lidar e o uso do Socket.IO para mostrar as novas mensagens em real time!

## :thinking: Como rodar o projeto?

1. Criar arquivo .env na raiz do projeto com 3 variáveis:

   <div style="margin-bottom: 12px;">

   ##### JWT_SECRET

   1. Entre em um site [MD5 Generator](https://www.md5hashgenerator.com/) e gere um hash com um texto, por exemplo **nlwheatnode**
      2.Copie esse hash e coloque na variável

   ##### GITHUB_CLIENT_ID e GITHUB_CLIENT_SECRET

   1. Faça o login no github e acesse Settings >> Developer settings >> OAuth Apps >> New OAuth App:
   2. Preencha os campos da seguinte forma:
      <strong>Application name: </strong> Coloque o que achar melhor
      <strong>Homepage URL: </strong> http://localhost:4000
      <strong>Authorization callback URL: </strong> http://localhost:4000/signin/callback
   3. Coloque o Client ID no GITHUB_CLIENT_ID, e pegar o GITHUB_CLIENT_SECRET basta clicar em Generate a new client secret
   </div>

2. Rodar `yarn` no terminal para instalar as dependências

3. Rodar `yarn prisma migrate dev` no terminal para rodar as migrations

4. Depois executar `yarn dev` para inicializar o servidor

5. Se no seu terminal você receber uma `Esta rodando na porta 4000`, significa que está tudo certo!
