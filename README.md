# Desafio Técnico – Low-Code (Java)

## 🌎 Contexto

Este desafio faz parte do processo seletivo para uma vaga de **desenvolvimento low-code**, utilizando **Java** como linguagem base.

O objetivo é avaliar a **capacidade de traduzir regras de negócio em lógica clara, legível e sustentável**, algo essencial no dia a dia de plataformas low-code.

Cenário proposto: **análise de dados de clientes para concessão de crédito**, a partir de um arquivo CSV.

---

## 🎯 Objetivo do desafio

Implementar uma solução em Java que **consuma um arquivo CSV contendo dados de clientes**, aplique **políticas de concessão de crédito** e gere um **novo arquivo CSV com o resultado da análise**.

O arquivo final deve conter, para cada cliente:

* A decisão da análise (aprovado ou reprovado)
* A **política de crédito atribuída**
* O **motivo principal** da decisão

Serão avaliados principalmente:

* Lógica de negócio
* Clareza e legibilidade do código

---

## 📦 Requisitos técnicos

### Linguagem e stack

* Linguagem: **Java**

### 🔧 Diferenciais (opcionais)

* Documentação clara
* Testes automatizados

---

## 🛠️ Problema de negócio

Você deve implementar uma solução em Java para **análise de clientes com objetivo de concessão de crédito**, a partir de um **arquivo CSV de entrada**, aplicando **políticas de crédito numeradas**.

Cada cliente analisado deve resultar em:

* Resultado da análise: **aprovado** ou **reprovado**
* **Política aplicada** (ex.: `politica_1`, `politica_2`, etc.)
* **Motivo principal** que levou à decisão

---

### 📄 Arquivo de entrada (CSV)

O desafio parte de um arquivo CSV, [clientes_analise.csv](clientes_analise.csv), contendo os dados dos clientes. O arquivo possui as seguintes colunas:

```
id,Nome,Idade,Renda,Meses Relacionamento,Score,Inadimplente
```

Descrição dos campos:

* `id`: identificador do cliente
* `Nome`: nome do cliente
* `Idade`: idade em anos
* `Renda`: renda mensal
* `Meses Relacionamento`: tempo de relacionamento com a instituição (em meses)
* `Score`: score de crédito (0 a 1000)
* `Inadimplente`: indica se o cliente possui inadimplência ativa (`true` ou `false`)

---

### 📄 Arquivo de saída (CSV)

A solução deve gerar um **novo arquivo CSV** contendo o resultado da análise de crédito para os clientes processados.

O arquivo de saída deve conter, no mínimo, as seguintes colunas:

```
id,Nome,Resultado,PoliticaAplicada,Motivo
```

Onde:

* `Resultado`: `APROVADO` ou `REPROVADO`
* `PoliticaAplicada`: identificador da política aplicada (ex.: `politica_3`)
* `Motivo`: descrição objetiva do motivo da decisão

---

### 📐 Políticas de concessão de crédito

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
* Lógica de negócio clara e correta
* Boa nomenclatura de classes, métodos e variáveis
* Separação razoável de responsabilidades
* README explicando:

  * Como executar o projeto
  * Como informar o arquivo CSV de entrada
  * Como o arquivo CSV de saída é gerado
  * Decisões técnicas relevantes

---

## 📬 Entrega

* Envie o código em um repositório GitHub
* Inclua o README com instruções claras de execução
* Ao finalizar, envie o link do repositório para alguém da nossa equipe

---

Boa sorte no desafio! 🚀
