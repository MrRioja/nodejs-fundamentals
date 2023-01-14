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
