---
date: 2019-09-11
title: Integração API
description: API simples e poderosa para integrar pagamentos por boletos bancários em seu site ou aplicação
categories:
  - integração
type: Document
set: integracao
set_order: 1
---

O Padmoney oferece aos desenvolvedores uma API simples e poderosa em REST para integrar pagamentos por boletos bancários em seu site ou aplicação.

## API Padmoney

Acesse a [Documentação da API do Padmoney](https://developers.padmoney.com) e encontre uma documentação completa para ajudar os desenvolvedores na integração com o Padmoney.

### Endpoint da API

A URL Base da API é https://api.padmoney.com/v2/.

Todas as requisições devem usar o schema `https` por questões de segurança.

### Autenticação

Atualmente é possível autenticar na API do Padmoney usando Token de Acesso. Para poder usar a autenticação via Token de Acesso, você precisa gerar o seu Token, onde será necessário informar uma Chave de Segurança, nas configurações da sua conta.

Após a geração do Token, com a Chave de Segurança e o Token em mãos, basta enviar no header da requisição essa informações.

Exemplo de requisição autenticada (onde `UGFkbW9uZXk=` é o Token de Acesso do usuário e `P@dm0n3y` é a chave de segurança):

```
GET /v2/ping
Padmoney-Token: UGFkbW9uZXk
Padmoney-Token-Secret: P@dm0n3y
```

