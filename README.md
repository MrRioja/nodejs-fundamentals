# Fundamentos do NodeJS - Ignite v2023

<p align="center">
  <img src="https://img.shields.io/static/v1?label=nodejs&message=fundamentals&color=blueviolet&style=for-the-badge"/>
  <img src="https://img.shields.io/github/license/MrRioja/nodejs-fundamentals?color=blueviolet&logo=License&style=for-the-badge"/>
  <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/MrRioja/nodejs-fundamentals?color=blueviolet&logo=JavaScript&logoColor=white&style=for-the-badge">
  <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/MrRioja/nodejs-fundamentals?color=blueviolet&style=for-the-badge">
</p>

<p align="center">
  <a href="#sobre">Sobre</a> •
  <a href="#fundamentos-do-nodejs">Fundamentos do NodeJS</a> •
  <a href="#instalação">Instalação</a> •
  <a href="#tecnologias">Tecnologias</a> •
  <a href="#autor">Autor</a>
</p>

## Sobre

Projeto I do bootcamp Ignite da [RocketSeat](https://www.rocketseat.com.br/) na versão lançada da trilha 2023. No primeiro módulo foi desenvolvido uma API RESTful com NodeJS focada nos fundamentos da tecnologia, sem frameworks ou bibliotecas externas.

## Fundamentos do NodeJS

No primeiro projeto da trilha de NodeJS v2023 foi construída uma API simples porém utilizando os recursos nativos do NodeJS.

O conteúdo aborda módulos internos do NodeJS como HTTP, Crypto e File System e sobre fundamentos HTTP como requests, respondes, headers, status code, route e query parameters, etc. Também possuem profundidade em Streams no NodeJS e como aplica-las para realizarmos operações assíncronas e parciais em nosso back-end.

Como o objetivo é entender o que os famosos frameworks fazem por debaixo dos panos, a API é simples e é composta pelas rotas abaixo:

<details>
  <summary>GET <code>/users</code></summary>
  <br>
  Rota para listar os usuários cadastrados. Seu retorno será um JSON com um array contendo os objetos de todos os usuários cadastrados.
</details>

<details>
  <summary>POST <code>/users</code></summary>
  <br>
  Rota para cadastrar um novo usuário. O corpo da requisição é semelhante ao exemplo abaixo e a rota não retornará nada além do status code <code>201</code>.
  <br>
  <pre>
    <code>
      {
        "name": "John Doe",
        "email": "johndoe@example.com"
      }
    </code>
  </pre>
</details>

<details>
  <summary>PUT <code>/users/{userId}</code></summary>
  <br>
  Rota para atualizar o cadastro de um usuário. A rota recebe como parâmetro o id do usuário a ser atualizado e o corpo da requisição é semelhante ao exemplo abaixo e substituirá os dados preenchidos anteriormente. A rota não retornará nada além do status code <code>204</code>.
  <br>
  <pre>
    <code>
      {
        "name": "John Doe",
        "email": "johndoe@example.com"
      }
    </code>
  </pre>
</details>

<details>
  <summary>DELETE <code>/users/{userId}</code></summary>
  <br>
  Rota para remover o cadastro de um usuário. A rota recebe como parâmetro o id do usuário a ser excluído. A rota não retornará nada além do status code <code>204</code>.
</details>

## Instalação

Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:
[Git](https://git-scm.com), [NodeJS](https://nodejs.org/en/).
Além disso é bom ter um editor para trabalhar com o código como [VSCode](https://code.visualstudio.com/).

### 🎲 Rodando o Back End (servidor)

```bash
# Clone este repositório
$ git clone git@github.com:MrRioja/nodejs-fundamentals.git

# Acesse a pasta do projeto no terminal/cmd
$ cd nodejs-fundamentals

# Execute a aplicação em modo de desenvolvimento
$ npm run dev
# Caso prefira usar o Yarn execute o comando abaixo
$ yarn dev

# O servidor inciará na porta 3333 - acesse <http://localhost:3333>
```

## Tecnologias

<img src="https://profilinator.rishav.dev/skills-assets/nodejs-original-wordmark.svg" alt="Node.js" height="75" />

## Autor

<div align="center">
<img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/55336456?v=4&h=100&w=100&fit=cover&mask=circle&maxage=7d" />
<h1>Luiz Rioja</h1>
<strong>Backend Developer</strong>
<br/>
<br/>

<a href="https://linkedin.com/in/luizrioja" target="_blank">
<img alt="LinkedIn" src="https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>

<a href="https://github.com/mrrioja" target="_blank">
<img alt="GitHub" src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white"/>
</a>

<a href="mailto:lulyrioja@gmail.com?subject=Fala%20Dev" target="_blank">
<img alt="Gmail" src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
</a>

<a href="https://api.whatsapp.com/send?phone=5511933572652" target="_blank">
<img alt="WhatsApp" src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white"/>
</a>

<a href="https://join.skype.com/invite/tvBbOq03j5Uu" target="_blank">
<img alt="Skype" src="https://img.shields.io/badge/SKYPE-%2300AFF0.svg?style=for-the-badge&logo=Skype&logoColor=white"/>
</a>

<br/>
<br/>
</div>
