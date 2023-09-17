
<h1 align="center">Desafio 01 - Conceitos do Node.js</h1>


<p align="center">
  <img alt="Rocketseat Education" src="https://avatars.githubusercontent.com/u/69590972?s=200&v=4" width="100px" />
</p>

<p align="center">
  <img src="https://img.shields.io/static/v1?label=Rocketseat&message=Education&color=8257e5&labelColor=202024" alt="Rocketseat Project" />
  <a href="LICENSE"><img  src="https://img.shields.io/static/v1?label=License&message=MIT&color=8257e5&labelColor=202024" alt="License"></a>
</p>


<h1 align="center">Desafio 02 - Trabalhando com Middlewares</h1>

## 🚀 O que é e o propósito do projeto

Este projeto faz parte do Desafio 02 do Bootcamp Ignite da Rocketseat, focado em aprofundar o conhecimento sobre middlewares no Express. O objetivo é consolidar os conceitos adquiridos até o momento.

A aplicação gerencia tarefas (*todos*) para usuários, permitindo a criação, listagem, atualização e exclusão de tarefas, além de operações relacionadas a usuários.

## 💻 Tecnologias

- [Node.js](https://nodejs.org/)
- [Express](https://expressjs.com/)
- [UUID](https://github.com/uuidjs/uuid)
- ...

## 🔌 Middlewares da aplicação

Neste desafio, o foco é nos middlewares, que desempenham funções cruciais para garantir o funcionamento correto da aplicação. Aqui está uma breve descrição de cada middleware:

### checksExistsUserAccount

Valida a existência de um usuário com base no `username` passado no header da requisição. Se existir, repassa o usuário para `request.user` e chama a função `next`.

### checksCreateTodosUserAvailability

Verifica se o usuário pode criar um novo *todo* com base no plano (grátis ou Pro) e na quantidade de *todos* que possui. Permite a criação se estiver no plano grátis e tiver menos de 10 *todos* ou se estiver no plano Pro.

### checksTodoExists

Valida se o *todo* pertence ao usuário, com base no `username` do header e no `id` do *todo* passado nos parâmetros. Se válido, passa o *todo* e o usuário para `request.todo` e `request.user`, respectivamente, e chama a função `next`.

### findUserById

Localiza um usuário com base no `id` fornecido nos parâmetros da rota. Se encontrado, repassa o usuário para `request.user` e chama a função `next`.

## Especificação dos testes

Os testes avaliam o funcionamento correto dos middlewares e estão detalhadamente descritos no [arquivo de especificação dos testes](https://link_para_especificacao_dos_testes).

...

## 🛠️ Como usar

1. Clone este repositório.
2. Instale as dependências com o comando: `yarn`.
3. Rode a aplicação com o comando: `yarn dev`.
4. A aplicação estará disponível em: `http://localhost:3333`.

## 📝 Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.


Feito com 💜 por Maxson Almeida 👋

[GitHub](https://github.com/maxsonferovante)
[LinkedIn](https://www.linkedin.com/in/maxson-almeida-501065260/)
