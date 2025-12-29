# Desafio Técnico – Low-Code (Java)

## 🌎 Contexto

Este desafio faz parte do processo seletivo para uma vaga de **desenvolvimento low-code**, utilizando **Java** como linguagem base.

O objetivo não é avaliar conhecimento profundo de frameworks ou arquitetura avançada, mas sim a **capacidade de traduzir regras de negócio em lógica clara, legível e sustentável**.

Cenário proposto: **análise de dados de clientes para concessão de crédito**.

---

## 🎯 Objetivo do desafio

Implementar uma solução em Java que avalie **clientes** com base em **políticas de concessão de crédito**, retornando a decisão de aprovação ou reprovação, bem como o motivo da decisão.

Serão avaliados principalmente:

* Lógica de negócio
* Clareza e legibilidade do código

---

## 📦 Requisitos técnicos

### Linguagem e stack

* Linguagem obrigatória: **Java**
* Uso de **frameworks**: **permitido, mas não obrigatório**

  * Fique à vontade para utilizar o framework de sua preferência
  * Não há exigência de padrões ou estruturas específicas

### Persistência de dados

  * [Docker Compose (preferencial)](docker-compose.yaml)
  * Supabase
  * Fly.io
  * MongoDB Atlas
  * Outros serviços

> Caso utilize algo diferente do Docker Compose disponibilizado, **documente claramente no README** como executar o projeto.

### 🔧 Diferenciais (opcionais)

* Documentação
* Testes automatizados
* Deploy da aplicação em algum provedor
* Uso de frameworks e dependências externas

---

## 🛠️ Problema de negócio

Você deve modelar e implementar a análise de **clientes** para **concessão de crédito**, com base em políticas definidas por você.

Cada cliente analisado deve resultar em:

* Aprovado ou reprovado
* Um motivo claro para a decisão

### Exemplos de critérios

Você tem liberdade para definir as regras, desde que façam sentido no contexto de crédito. Exemplos:

* Histórico financeiro do cliente
* Renda ou capacidade de pagamento
* Score ou classificação de risco
* Relacionamento prévio com a instituição
* Perfil do cliente pode impactar a política de crédito

> O mais importante não é **quais regras** você cria, mas **como elas são implementadas e organizadas**.

---

## 📄 O que esperamos da solução

* Código organizado e fácil de entender
* Regras de negócio claras
* Boa nomenclatura de classes, métodos e variáveis
* Separação razoável de responsabilidades
* README explicando:

  * Como executar o projeto
  * Dependências
  * Decisões técnicas relevantes

---

## 📬 Entrega

* Envie o código em um repositório GitHub
* Não esqueça do README com instruções claras de execução e demais pontos importantes da solução
* Ao finalizar, envie o link do repositório para alguém da nossa equipe

---

Boa sorte no desafio! 🚀
