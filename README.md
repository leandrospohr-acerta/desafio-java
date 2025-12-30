# Desafio Técnico – Low-Code (Java)

## 🌎 Contexto

Este desafio faz parte do processo seletivo para uma vaga de **desenvolvimento low-code**, utilizando **Java** como linguagem base.

O objetivo não é avaliar a **capacidade de traduzir regras de negócio em lógica clara, legível e sustentável**.

Cenário proposto: **análise de dados de clientes para concessão de crédito**.

---

## 🎯 Objetivo do desafio

Implementar uma solução em Java que avalie **clientes** com base em **políticas de concessão de crédito**, retornando a decisão de aprovação ou reprovação, a politíca atribuída, bem como o motivo da decisão.

Serão avaliados principalmente:

* Lógica de negócio
* Clareza e legibilidade do código

---

## 📦 Requisitos técnicos

### Linguagem e stack

* Linguagem: **Java**

### 🔧 Diferenciais (opcionais)

* Documentação
* Testes automatizados

---

## 🛠️ Problema de negócio

Você deve implementar uma solução em Java para **análise de clientes com objetivo de concessão de crédito**, aplicando **políticas de crédito numeradas**.

Cada cliente analisado deve resultar em:

* Resultado da análise: **aprovado** ou **reprovado**
* **Política aplicada** (ex.: `politica_1`, `politica_2`, etc.)
* **Motivo principal** que levou à decisão

### Dados do cliente

Cada cliente possui, no mínimo, as seguintes informações:

* Idade
* Renda mensal
* Tempo de relacionamento com a instituição (em meses)
* Score de crédito (0 a 1000)
* Indicador de inadimplência ativa (boolean)

Você pode modelar esses dados da forma que considerar mais adequada, desde que todas as informações acima sejam consideradas na análise.

---

### Políticas de concessão de crédito

A análise deve aplicar **exatamente uma política por cliente**, seguindo **rigorosamente a ordem de prioridade abaixo**.
A primeira política cujo critério seja atendido deve ser aplicada, encerrando a análise.

**Política 1 (`politica_1`) — Inadimplência ativa**

* Clientes com inadimplência ativa devem ser **reprovados automaticamente**.

**Política 2 (`politica_2`) — Score insuficiente**

* Clientes com score de crédito **inferior a 500** devem ser **reprovados**.

**Política 3 (`politica_3`) — Renda mínima**

* Clientes com renda mensal **inferior a um valor mínimo**, definido por você, devem ser **reprovados**.

**Política 4 (`politica_4`) — Relacionamento insuficiente**

* Clientes com **menos de 6 meses de relacionamento** com a instituição devem ser **reprovados**.

**Política 5 (`politica_5`) — Aprovação padrão**

* Clientes que não se enquadram em nenhuma das políticas anteriores devem ser **aprovados**.

O resultado da análise deve sempre indicar **qual política foi aplicada**, inclusive no caso de aprovação.

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
