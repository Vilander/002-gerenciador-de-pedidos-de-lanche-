# 002-gerenciador-de-pedidos-de-lanche

## Situação de Aprendizagem 2: Desenvolvimento de Estruturas de Dados e Lógica CRUD

Objetivo: Criação de modelos de dados (classes/objetos) para o Back-End. Implementação da lógica de tratamento de requisições (POST/GET) e manipulação de dados (CRUD - Criar, Ler, Atualizar, Deletar), utilizando Node.js/Express.

## Gerenciador de Pedidos de Lanche (In-Memory)

Descrição: Desenvolver uma API Node.js/Express que gerencie uma lista de pedidos de lanche (Armazenamento em memória, sem banco de dados ainda). A API deve ter rotas para: (C) Criar um novo pedido (POST), (R) Listar todos os pedidos e buscar um pedido por ID (GET), (U) Atualizar o status de um pedido (PATCH ou PUT), e (D) Cancelar um pedido (DELETE). Isso exige a criação de classes ou objetos para modelar o pedido e o tratamento correto das requisições HTTP.

---

# Iniciando um projeto

1. Abrir terminal (`CTRL+J`). Alterar para cmd
2. iniciar projeto: `npm init` ou `npm init -y`
3. Será gerado package.json onde pode alterar os dados
4. Instalar express.js para trabalhar com os verbos HTTP (`GET, POST, PUT, DELETE`)
   - `npm install express` ou `npm i express`
5. Criar arquivo `index.js`

```javascript
const express = require("express");
const app = express();

app.get("/", function (req, res) {
  res.send("Hello World");
});

app.listen(3000);
```

6. Executar: digitar no terminal `node index.js`
7. Abrir //localhost:3000
