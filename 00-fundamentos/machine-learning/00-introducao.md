# 🤖 Introdução ao Machine Learning

## 📌 O que é

Machine Learning (ML) é uma área da Inteligência Artificial (Artificial Intelligence - AI) que permite que sistemas **aprendam padrões a partir de dados** e façam previsões ou tomem decisões **sem serem explicitamente programados**.

<img width="448" height="447" alt="image" src="https://github.com/user-attachments/assets/fc202791-6eba-41e5-bf99-08d7337810e6" />

Em vez de seguir regras fixas definidas por um desenvolvedor, um modelo de ML aprende com exemplos e utiliza esse conhecimento para realizar previsões sobre novos dados.

---

## 🎯 Quando usar

O Machine Learning é indicado quando:

- Há **grande volume de dados** disponível
- É difícil definir regras fixas para resolver um problema
- É necessário identificar padrões ou fazer previsões

### Exemplos de uso

- Previsão de preços
- Previsão de demanda
- Classificação de e-mails como spam
- Detecção de fraudes
- Sistemas de recomendação
- Análise de comportamento de clientes

---

## ⚙️ Como funciona

O desenvolvimento de um modelo de Machine Learning segue, de forma geral, o seguinte fluxo:

1. Coleta de dados
2. Preparação dos dados
3. Escolha do algoritmo
4. Treinamento do modelo
5. Avaliação
6. Iteração (melhoria contínua)
7. Inferência (uso em produção)

📌 Esse processo é iterativo: caso o modelo não apresente o desempenho esperado, normalmente é necessário voltar às etapas anteriores para melhorar os dados, ajustar parâmetros ou escolher outro algoritmo.

---

## 🧠 Conceitos importantes

### 📊 Dados de treinamento (Training Data)

São os dados utilizados para ensinar o modelo durante o treinamento.

É uma das etapas mais importantes do Machine Learning, pois a qualidade dos dados influencia diretamente a qualidade das previsões.

#### Problemas comuns

- Dados incompletos
- Dados inconsistentes
- Dados duplicados
- Dados enviesados (Bias)

📌 Um algoritmo excelente não consegue compensar dados de baixa qualidade.

---

### 🏷️ Dados rotulados vs dados não rotulados

Os dados utilizados em Machine Learning podem ser classificados em dois grupos.

#### Dados rotulados (Labeled Data)

Possuem a entrada e a resposta correta (**label**).

Exemplos:

- Imagem → "gato"
- E-mail → "spam"
- Produto → "eletrônico"

São utilizados principalmente no **aprendizado supervisionado (Supervised Learning)**.

---

#### Dados não rotulados (Unlabeled Data)

Contêm apenas os dados de entrada, sem a resposta correta.

Exemplos:

- Coleção de imagens sem classificação
- Lista de clientes sem segmentação
- Textos sem categoria

São utilizados principalmente no **aprendizado não supervisionado (Unsupervised Learning)**.

---

### 🧱 Tipos de dados

Os modelos de Machine Learning podem trabalhar com diferentes tipos de dados.

#### 📋 Dados estruturados (Structured Data)

Possuem uma estrutura organizada, normalmente em linhas e colunas.

Exemplos:

- Bancos de dados relacionais
- Arquivos CSV
- Planilhas

Subtipos comuns:

- Dados tabulares
- Séries temporais (Time Series)

---

#### 🧩 Dados não estruturados (Unstructured Data)

Não seguem um formato fixo.

Exemplos:

- Texto
- Imagens
- Áudio
- Vídeo

Em geral, exigem técnicas mais avançadas para processamento.

---

## 📌 Garbage In, Garbage Out (GIGO)

Um dos princípios mais importantes do Machine Learning é:

> **Garbage In, Garbage Out**

Isso significa que **um modelo é tão bom quanto os dados utilizados para treiná-lo**.

Mesmo utilizando algoritmos sofisticados, dados incorretos, incompletos ou enviesados produzirão resultados ruins.

📌 Na prática, a qualidade dos dados costuma ter um impacto maior do que a escolha do algoritmo.

---

## 💰 Modelo de cobrança (conceitual)

No contexto da AWS, normalmente os custos de Machine Learning estão relacionados ao processamento utilizado.

Os dois principais momentos que geram custos são:

- **Treinamento:** normalmente possui maior custo computacional
- **Inferência:** gera custo contínuo enquanto o modelo está em uso

📌 Em muitas aplicações, o modelo é treinado poucas vezes, mas realiza inferências continuamente.

---

## 🔒 Segurança (conceitual)

A segurança também faz parte de projetos de Machine Learning.

Alguns riscos incluem:

- Vazamento de dados
- Uso de dados sensíveis
- Dados enviesados (Bias)
- Acesso não autorizado aos modelos

Boas práticas incluem:

- Controle de acesso
- Proteção dos dados
- Monitoramento contínuo
- Governança dos modelos

---

## 🧠 Conceitos importantes para prova

- Machine Learning aprende padrões a partir dos dados
- O modelo aprende com exemplos, e não com regras programadas manualmente
- A qualidade dos dados é um dos fatores mais importantes para o sucesso do modelo
- Dados rotulados são usados principalmente em aprendizado supervisionado
- Dados não rotulados são usados principalmente em aprendizado não supervisionado
- Dados podem ser estruturados ou não estruturados
- **Garbage In, Garbage Out (GIGO)** é um conceito fundamental em Machine Learning
- Na AWS, treinamento e inferência são as principais fontes de custo relacionadas ao ML

---

## ⚠️ Pegadinhas comuns

- Machine Learning **não substitui completamente regras de negócio**
- Mais dados **não significam necessariamente um modelo melhor**
- O melhor algoritmo não compensa dados de baixa qualidade
- Dados rotulados e dados estruturados são conceitos diferentes
- Dados não estruturados podem ser utilizados em Machine Learning
- Um modelo aprende padrões; ele não "entende" os dados como um ser humano

---

## 🔁 Resumo rápido

- Machine Learning aprende padrões a partir de dados
- Dados de qualidade são fundamentais
- O processo de ML envolve coleta, preparação, treinamento, avaliação e inferência
- Existem dados rotulados e não rotulados
- Os dados podem ser estruturados ou não estruturados
- O princípio **Garbage In, Garbage Out** reforça a importância da qualidade dos dados
- Na AWS, os principais custos costumam estar relacionados ao treinamento e à inferência

---

## 📌 Status de aprendizado

- [ ] Entendo o que é Machine Learning
- [ ] Sei quando utilizar Machine Learning
- [ ] Entendo o fluxo geral de um projeto de ML
- [ ] Sei diferenciar dados rotulados e não rotulados
- [ ] Sei diferenciar dados estruturados e não estruturados
- [ ] Entendo o conceito de **Garbage In, Garbage Out (GIGO)**
- [ ] Conheço os principais aspectos de segurança e custos em Machine Learning
