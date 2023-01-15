# Notes - NodeJS fundamentals

- Para alterar o tipo de importação de CommonJS para ESModules é necessário adicionar a chave abaixo no `package.json`:

```json
"type": "module"
```

> ℹ Ao utilizar esse type, devemos especificar a extensão ao importar um arquivo de um modulo.

- As versões mais atuais do Node já suportam a flag `--watch` em scripts para sincronizar alterações do código sem ter que reiniciar o servidor. Basta criar um script no `package.json` como abaixo:

```json
"scripts": {
  "dev": "node --watch src/server.js"
}
```

- Para indicar que a resposta está em um formato especifico devemos setar o header `Content-type` com o valor deseja, como por exemplo `application/json` para JSON.

- No NodeJS temos dois principais tipos de streams: `Readable` e `Writable`. As streams são utilizadas para processamento de dados em paralelo e não reconhecem tipos primitivos, os quais devem ser transformados em Buffer antes de serem enviados para consumo. Também temos as streams do tipo `Transform`, que recebem dados e os repassam após algum tipo de transformação.

- Em uma API REST temos três tipos de parâmetros:

  - **Query Parameters:** Utilizada quando precisamos ter uma URL stateful como por exemplo para armazenar estado de paginação, filtros ou quando teremos parâmetros não obrigatórios. A URL a seguir é um exemplo do uso desse tipo de parâmetro:
    `GET http://localhost:3333/users?userId=1&name=Diego`

  - **Route Parameters:** Utilizada quando precisamos identificar um recurso para uma determinada ação. A URL a seguir é um exemplo do uso desse tipo de parâmetro:
    `GET http://localhost:3333/users/1`

  - **Request body:** Utilizada quando precisamos informar diversos dados e tipo de passagem de parâmetro comumente usado em formulários. A URL a seguir é um exemplo do uso desse tipo de parâmetro, a URL não sofre alteração pois os parâmetros são informados no corpo da requisição:
    `POST http://localhost:3333/users`
