---
layout: default
title: Integração
nav_order: 2
---

# Integração
{: .no_toc }

O Padmoney oferece aos desenvolvedores uma API simples e poderosa em REST para integrar pagamentos por boletos bancários em seu site ou aplicação.
{: .fs-6 .fw-300 }

{: .no_toc .text-delta }

1. TOC
{:toc}

---


Acesse a [Documentação da API do Padmoney](https://developers.padmoney.com) e encontre uma documentação completa para ajudar os desenvolvedores na integração com o Padmoney.

## API Padmoney

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

## Módulos e Plugins

Existem módulos prontos para integrar ao Padmoney sem a necessidade de desenvolver a integração. 

### HOSTMGR

O módulo de integração para HOSTMGR é o oficial e disponibilizado de forma nativa no sistema. Conheça o HOSTMGR em [www.hostmgr.com.br](https://www.hostmgr.com.br/).

### WHMCS

[WHMCS](https://www.whmcs.com/), abreviação de WebHost Manager Complete Solution, é um sistema de gestão de clientes, administração financeira e prestação de suporte, com integração a diversos painéis de controle, e utilizado em empresas de web hosting.

Atualmente o Padmoney conta com dois parceiros para WHMCS. Fique a vontade para conhece-los através dos links:

- [https://www.edvan.com.br/financeiro/padmoney.php](https://www.edvan.com.br/financeiro/padmoney.php)
- [https://gofas.net/whmcs/modulo-padmoney-boleto-para-whmcs/](https://gofas.net/whmcs/modulo-padmoney-boleto-para-whmcs/)
