# 🧠 Tipos de Machine Learning

## 📌 O que são

Os **tipos de Machine Learning** definem como um modelo aprende a partir dos dados.

A escolha do tipo depende principalmente de:

- Existência ou não de dados rotulados
- Objetivo do problema
- Forma como o modelo recebe feedback

Os quatro principais tipos são:

- 🟢 Aprendizado supervisionado (Supervised Learning)
- 🟡 Aprendizado não supervisionado (Unsupervised Learning)
- 🔵 Aprendizado por reforço (Reinforcement Learning)
- 🟣 Aprendizado semi-supervisionado (Semi-supervised Learning)

---

## 🟢 Aprendizado supervisionado (Supervised Learning)

<img width="849" height="420" alt="image" src="https://github.com/user-attachments/assets/f4867291-31fa-4d14-b0d5-12a250f57b76" />

No aprendizado supervisionado, o modelo é treinado utilizando **dados rotulados**, ou seja, cada exemplo possui a entrada e a resposta correta.

O objetivo é aprender a relação entre entrada e saída para realizar previsões sobre novos dados.

### Características

- Usa dados rotulados
- Aprende a relação entre entrada e saída
- Faz previsões para novos dados
- É o tipo mais utilizado em aplicações de Machine Learning

### Principais aplicações

- Classificação
- Regressão

---

### 🏷️ Classificação (Classification)

A classificação prevê **categorias ou classes**.

Exemplos:

- Spam ou não spam
- Fraude ou transação legítima
- Diagnóstico positivo ou negativo

### Casos de uso

- Detecção de fraudes
- Classificação de imagens
- Classificação de documentos
- Retenção de clientes

📌 O resultado pertence a uma categoria previamente definida.

---

### 📈 Regressão (Regression)

A regressão prevê **valores numéricos contínuos**.

Exemplos:

- Preço de imóveis
- Temperatura
- Consumo de energia
- Crescimento populacional

### Casos de uso

- Previsão do tempo
- Mercado financeiro
- Previsão de demanda
- Popularidade de anúncios

📌 O resultado é um valor numérico.

---

## 🟡 Aprendizado não supervisionado (Unsupervised Learning)

<img width="444" height="541" alt="image" src="https://github.com/user-attachments/assets/ab023048-9a2a-44b6-919f-4285c4f7ccc4" />

No aprendizado não supervisionado, o modelo recebe **dados sem rótulos**.

Seu objetivo é descobrir padrões, relacionamentos ou estruturas existentes nos dados.

### Características

- Não utiliza respostas corretas
- Descobre padrões automaticamente
- Organiza dados semelhantes

### Principais aplicações

- Clustering
- Redução de dimensionalidade

---

### 🧩 Agrupamento em clusters (Clustering)

O clustering agrupa dados semelhantes sem que existam categorias previamente definidas.

Exemplos:

- Segmentação de clientes
- Marketing direcionado
- Sistemas de recomendação

### Objetivo

Encontrar grupos naturais dentro dos dados.

📌 O algoritmo cria os grupos automaticamente.

---

### 📉 Redução de dimensionalidade (Dimensionality Reduction)

A redução de dimensionalidade diminui a quantidade de atributos utilizados pelo modelo, preservando as informações mais relevantes.

### Casos de uso

- Visualização de dados
- Compressão de dados
- Descoberta de padrões
- Redução da complexidade do modelo

📌 Uma técnica bastante conhecida é o **PCA (Principal Component Analysis)**.

---

## 🔵 Aprendizado por reforço (Reinforcement Learning)

O aprendizado por reforço é baseado em **tentativa e erro**.

O modelo aprende interagindo com um ambiente e recebe recompensas quando toma boas decisões e penalidades quando toma decisões inadequadas.

### Componentes

- Agente
- Ambiente
- Ações
- Recompensas

### Características

- Aprende continuamente
- Não depende de um conjunto tradicional de dados rotulados
- Busca maximizar a recompensa ao longo do tempo

### Casos de uso

- Robótica
- Jogos
- Veículos autônomos
- Otimização de processos

---

### 🏎️ Exemplo: AWS DeepRacer

<img width="509" height="395" alt="image" src="https://github.com/user-attachments/assets/50a2cba9-4a5b-4fc7-9f36-5a69fe51eb89" />

O **AWS DeepRacer** é um dos exemplos mais conhecidos de aprendizado por reforço na AWS.

Nesse cenário:

- **Agente:** carro virtual
- **Ambiente:** pista virtual
- **Objetivo:** completar a pista o mais rápido possível sem sair dela

A cada volta, o agente aprende com seus erros e melhora sua estratégia.

📌 O aprendizado acontece por meio do feedback recebido durante as interações.

---

## 🟣 Aprendizado semi-supervisionado (Semi-supervised Learning)

O aprendizado semi-supervisionado combina características dos modelos supervisionados e não supervisionados.

Utiliza:

- Poucos dados rotulados
- Muitos dados não rotulados

É útil quando rotular dados é caro, demorado ou exige especialistas.

### Casos de uso

- Diagnóstico médico
- Classificação de imagens
- Reconhecimento de fala
- Processamento de documentos

---

## 🔁 Comparações importantes

### Dados rotulados vs dados não rotulados

| Dados rotulados | Dados não rotulados |
|-----------------|---------------------|
| Possuem resposta correta | Não possuem resposta correta |
| Utilizados no aprendizado supervisionado | Utilizados no aprendizado não supervisionado |
| Mais caros de produzir | Mais baratos de obter |
| Geralmente proporcionam maior precisão | Mais exploratórios |

---

### Tipos de Machine Learning

| Tipo | Usa rótulos? | Objetivo |
|------|--------------|----------|
| Supervisionado | ✅ Sim | Fazer previsões |
| Não supervisionado | ❌ Não | Descobrir padrões |
| Reforço | ❌ Não diretamente | Aprender por tentativa e erro |
| Semi-supervisionado | Parcialmente | Combinar poucos rótulos com muitos dados |

---

### Classificação vs Regressão

| Classificação | Regressão |
|--------------|-----------|
| Prevê categorias | Prevê valores numéricos |
| Resultado discreto | Resultado contínuo |
| Spam ou não spam | Preço de um imóvel |

---

### Clustering vs Classificação

| Clustering | Classificação |
|------------|---------------|
| Não supervisionado | Supervisionado |
| Não possui rótulos | Utiliza rótulos |
| Descobre grupos | Prevê categorias existentes |

---

## 🧠 Conceitos importantes para prova

- Existem quatro principais tipos de Machine Learning
- Aprendizado supervisionado utiliza dados rotulados
- Aprendizado não supervisionado utiliza dados não rotulados
- Classificação prevê categorias
- Regressão prevê valores numéricos
- Clustering encontra grupos naturalmente nos dados
- Redução de dimensionalidade reduz atributos preservando informações relevantes
- Aprendizado por reforço aprende por tentativa e erro
- O AWS DeepRacer é um exemplo clássico de Reinforcement Learning
- O aprendizado semi-supervisionado combina poucos dados rotulados com muitos dados não rotulados

---

## ⚠️ Pegadinhas comuns

- Aprendizado não supervisionado **não significa que o modelo não aprende**
- Classificação não prevê valores numéricos
- Regressão não classifica categorias
- Clustering não utiliza rótulos
- Reinforcement Learning não aprende a partir de um conjunto tradicional de dados rotulados
- Semi-supervisionado não significa "metade supervisionado e metade não supervisionado"; normalmente utiliza poucos dados rotulados e muitos não rotulados

---

## 🔁 Resumo rápido

- **Supervisionado:** usa dados rotulados para fazer previsões
- **Não supervisionado:** encontra padrões em dados sem rótulos
- **Reforço:** aprende por tentativa e erro utilizando recompensas
- **Semi-supervisionado:** combina poucos dados rotulados com muitos não rotulados
- Classificação prevê categorias
- Regressão prevê valores numéricos
- Clustering agrupa dados semelhantes
- Redução de dimensionalidade reduz a quantidade de atributos mantendo as informações mais importantes

---

## 📌 Status de aprendizado

- [ ] Sei diferenciar os principais tipos de Machine Learning
- [ ] Entendo quando utilizar aprendizado supervisionado
- [ ] Entendo quando utilizar aprendizado não supervisionado
- [ ] Sei diferenciar classificação e regressão
- [ ] Entendo o conceito de clustering
- [ ] Entendo o conceito de redução de dimensionalidade
- [ ] Sei como funciona o aprendizado por reforço
- [ ] Conheço o AWS DeepRacer como exemplo de Reinforcement Learning
- [ ] Entendo quando utilizar aprendizado semi-supervisionado
