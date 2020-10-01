# 🗂 Repositórios
Durante o bootcamp GoStack fomos desafiados em uma série de atividades a fim de comprovarmos nosso entendimento sobre o assunto. 
Neste primeiro desafio, tivemos que realizar a implementação de cadastro simples de repositórios, onde este é composto pelo backend, um Website e um app Mobile.

# 🔱 Estrutura
#### Backend:
A estrutura do backend é composta por 5 rotas que são dividas da seguinte maneira:
  - POST `/repositories`: A rota recebe `title, url e techs` dentro do corpo da requisição, sendo a URL o link para o github desse repositório. Ao cadastrar um novo projeto, ele deve ser armazenado dentro de um objeto no seguinte formato: `{ id: "uuid", title: 'Desafio Node.js', url: 'http://github.com/...', techs: ["Node.js", "..."], likes: 0 }`;

  - GET `/repositories`: Rota que lista todos os repositórios;

  - PUT `/repositories/:id`: Rota utilizada para alterar apenas o title, a url e as techs do repositório que possua o id igual ao id presente nos parâmetros da rota;

  - DELETE `/repositories/:id`: Rota para deletar o repositório com o id presente nos parâmetros da rota;

  - POST `/repositories/:id/like`: Rota responsável por aumentar o número de likes do repositório específico escolhido através do id presente nos parâmetros da rota, a cada chamada dessa rota, o número de likes é aumentado em 1;

#### Website:
O Website possui uma funcionalidade simples sendo possível, **Listar os repositórios da API**, **Adicionar um repositório a API** e **Remover um repositório da API**.

![Site](https://user-images.githubusercontent.com/8752639/94755182-03cb3d80-036a-11eb-9534-c0981e909747.PNG)

#### Mobile:
No aplicativo Mobile além de poder **Listar os repositórios da API** também é possivel **Curtir um repositório listado**.

![mobile](https://user-images.githubusercontent.com/8752639/94755195-10e82c80-036a-11eb-8aa2-d400697d3ae2.PNG)

# 💻 Tecnologias

#### Backend (NodeJS + JavaScript)
- Express
- CORS
- UUIDV4

#### Website (React + JavaScript)
- Axios
- React Dom
- React Scripts

#### Mobile (React Native + JavaScript)
- Axios

# 📣 Meta
Ronaldo Tadeu Murguero Junior - murguero.ronaldo@gmail.com
