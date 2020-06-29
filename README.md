### API NodeJs

Projeto para exercitar os conceitos básicos de uma API em NodeJS com funcionalidades de criar, listar, alterar e deletar repositórios. 
- Possui uma requisição extra para a adição de likes nos repositórios já criados.

## Tecnologias
- [Express](https://expressjs.com/pt-br/)
- [Jest](https://jestjs.io/)


### Rotas da aplicação

- **`POST /repositories`**: A rota deve receber `title`, `url` e `techs` dentro do corpo da requisição, sendo a URL o link para o github desse repositório. Ao cadastrar um novo projeto, ele deve ser armazenado dentro de um objeto no seguinte formato: `{ id: "uuid", title: 'Desafio Node.js', url: 'http://github.com/...', techs: ["Node.js", "..."], likes: 0 }`; Certifique-se que o ID seja um UUID, e de sempre iniciar os likes como 0.

- **`GET /repositories`**: Rota que lista todos os repositórios;

- **`PUT /repositories/:id`**: A rota deve alterar apenas o `title`, a `url` e as `techs` do repositório que possua o `id` igual ao `id` presente nos parâmetros da rota;

- **`DELETE /repositories/:id`**: A rota deve deletar o repositório com o `id` presente nos parâmetros da rota;

- **`POST /repositories/:id/like`**: A rota deve aumentar o número de likes do repositório específico escolhido através do `id` presente nos parâmetros da rota, a cada chamada dessa rota, o número de likes deve ser aumentado em 1;


## Instalações e usos

Clone ou faça o download desse repositório:

```
# Clone o repositório
$ git clone https://github.com/rodolforoc/api-node 
```

Dentro da pasta /api-node rode os seguintes comandos:

```
# Instale as dependencias
$ yarn

# Rode a API
$ yarn dev

# running on port 3333
```
