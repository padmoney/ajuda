---
date: 2019-09-12
title: Dúvidas Frequentes
description: Learn how to use collections to manage and organize related content
categories:
  - transferência
faq:
  - question: Após o pagamento do boleto, qual o tempo para que o valor esteja disponível em minha conta?
    answer: Após a liquidação da cobrança, o valor estará disponível em sua conta para transferência em 1 dia útil. Antes deste período, o valor aparecerá no seu extrato financeiro como "lançamentos futuros".
type: Document
set: transferencia
set_order: 1
---


<section class="faq">
	<ul>
		{% for item in page.faq %}
			<li><a href="#{{ item.question | slugify }}">{{ item.question }}</a></li>
		{% endfor %}
	</ul>

	{% for item in page.faq %}
		<h2 id="{{ item.question | slugify}}">{{ item.question }}<a class="header-link" href="#{{ item.question | slugify }}">#</a></h2>
		{{ item.answer | markdownify }}
	{% endfor %}
</section>
