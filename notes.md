# Notes - NodeJS fundamentals

- Para alterar o tipo de importação de CommonJS para ESModules é necessário adicionar a chave abaixo no `package.json`:

```json
"type": "module"
```

- As versões mais atuais do Node já suportam a flag `--watch` em scripts para sincronizar alterações do código sem ter que reiniciar o servidor. Basta criar um script no `package.json` como abaixo:

```json
"scripts": {
  "dev": "node --watch src/server.js"
}
```

- Para indicar que a resposta está em um formato especifico devemos setar o header `Content-type` com o valor deseja, como por exemplo `application/json` para JSON.

- No NodeJS temos dois principais tipos de streams: `Readable` e `Writable`. As streams são utilizadas para processamento de dados em paralelo e não reconhecem tipos primitivos, os quais devem ser transformados em Buffer antes de serem enviados para consumo. Também temos as streams do tipo `Transform`, que recebem dados e os repassam após algum tipo de transformação.
