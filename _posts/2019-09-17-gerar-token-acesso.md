---
date: 2019-09-11
title: Autenticação usando Token de Acesso
description: API simples e poderosa para integrar pagamentos por boletos bancários em seu site ou aplicação
categories:
  - integração
type: Document
set: integracao
set_order: 2
---


## Como funciona?

Para poder usar a autenticação via Token de Acesso, você precisa gerar e pegar o seu Token, onde será necessário informar uma Chave de Segurança, nas configurações da sua conta.

Após a geração do Token, com a Chave de Segurança e o Token em mãos, basta enviar no header da requisição essa informações.

Exemplo de requisição autenticada, onde:
- `JDJhJDEwJDlqamNHTjFrRDk4Y0NOdm90T09tSXV6NWVvLkg0RDA2SFlkRVJCYlZBRjdESndJUmJkbXlx` é o Token de Acesso, e 
- `Br3z0` é a chave de segurança

Exemplo de requisição usando Token de Acesso

```
GET /v2/ping
Padmoney-Token: JDJhJDEwJDlqamNHTjFrRDk4Y0NOdm90T09tSXV6NWVvLkg0RDA2SFlkRVJCYlZBRjdESndJUmJkbXlx
Padmoney-Token-Secret: Br3z0
```

## Como gerar o Token de Acesso?


#### 1 - Acessar o Padmoney

Primeiro é necessário [acessar sua conta no Padmoney](https://app.padmoney.com/), acessar as Configurações da Conta e clicar em Integração com API. Após seguir esses passos você verá a seguinte tela:

![Integração com API](/images/screenshots/token-acesso-1.png)

#### 2 - Chave de Segurança

Para gerar o Token de Acesso é necessário informar e confirmar uma Chave de Segurança.

Detalhe que essa Chave de Segurança NÃO DEVE ser sua senha de acesso ao Padmoney, pois assim você terá mais segurança na privacidade dos seus dados.

![Informa/confirma Chave de Segurança](/images/screenshots/token-acesso-2.png)

#### 3 - Gerar novo token

Após informar e confirmar sua Chave de Segurança, clique no botão Gerar novo token:

![Gerar novo token](/images/screenshots/token-acesso-3.png)

#### 4 - Token de Acesso

Feito isso seu Token de Acesso estará criado, ou atualizado, e pronto para ser usado.

![Token de Acesso criado](/images/screenshots/token-acesso-4.png)


Acesse a [Documentação da API do Padmoney](https://developers.padmoney.com) e encontre uma documentação completa para ajudar os desenvolvedores na integração com o Padmoney.
