<img alt="GoStack" src="https://storage.googleapis.com/golden-wind/bootcamp-gostack/header-desafios-new.png" />

<h2 align="center">
  Desafios Bootcamp GoStack
</h2>

<p align="center">
  <img alt="License" src="https://img.shields.io/badge/license-MIT-%2304D361">
  
  <img alt="Repository size" src="https://img.shields.io/github/repo-size/lucasbaquinoo/gostack-conceitos-nodejs">
  
  <a href="https://github.com/lucasbaquinoo/gostack-conceitos-nodejs/commits/master">
  <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/lucasbaquinoo/gostack-conceitos-nodejs">
 </a>
</p>

## :rocket: Tecnologias

Esse projeto foi desenvolvido com as seguintes tecnologias:

- [Node.js](https://nodejs.org/en/)
- [Express](https://expressjs.com/)
- [Nodemon](https://nodemon.io/)
- [Jest](https://jestjs.io/)
- [UUIDV4](https://www.npmjs.com/package/uuidv4)


## :rocket: Sobre o desafio

Essa será uma aplicação para armazenar repositórios do seu portfólio, que irá permitir a criação, listagem, atualização e remoção dos repositórios, e além disso permitir que os repositórios possam receber "likes".

## 🤔 Como rodar na sua máquina (passos)
1. Clone no diretório de sua preferência, digitando o comando: ` git clone https://github.com/lucasbaquinoo/gostack-conceitos-nodejs.git `
2. Abra o projeto e instale as dependências com o código: `npm install` ou `yarn`
3. Após a instalação, rode o projeto com: `npm run dev` ou `yarn dev`

### Rotas da aplicação

- **`POST /repositories`**: A rota deve receber `title`, `url` e `techs` dentro do corpo da requisição, sendo a URL o link para o github desse repositório. Ao cadastrar um novo projeto, ele deve ser armazenado dentro de um objeto no seguinte formato: `{ id: "uuid", title: 'Desafio Node.js', url: 'http://github.com/...', techs: ["Node.js", "..."], likes: 0 }`; Certifique-se que o ID seja um UUID, e de sempre iniciar os likes como 0.

- **`GET /repositories`**: Rota que lista todos os repositórios;

- **`PUT /repositories/:id`**: A rota deve alterar apenas o `title`, a `url` e as `techs` do repositório que possua o `id` igual ao `id` presente nos parâmetros da rota;

- **`DELETE /repositories/:id`**: A rota deve deletar o repositório com o `id` presente nos parâmetros da rota;

- **`POST /repositories/:id/like`**: A rota deve aumentar o número de likes do repositório específico escolhido através do `id` presente nos parâmetros da rota, a cada chamada dessa rota, o número de likes deve ser aumentado em 1;

## :memo: Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE.md) para mais detalhes.

---

Feito com ♥ by ME :wave: 
