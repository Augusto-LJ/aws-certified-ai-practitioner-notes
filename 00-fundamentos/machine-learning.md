# 🤖 Fundamentos de Machine Learning

## 📌 O que é

Machine Learning (ML) é uma área da inteligência artificial que permite que sistemas **aprendam padrões a partir de dados** e façam previsões ou tomem decisões **sem serem explicitamente programados**.

<img width="448" height="447" alt="image" src="https://github.com/user-attachments/assets/fc202791-6eba-41e5-bf99-08d7337810e6" />

---

## 🎯 Quando usar

- Quando há **grande volume de dados**
- Quando regras fixas são difíceis de definir
- Para:
  - Previsões (ex: preço, demanda)
  - Classificação (ex: spam vs não spam)
  - Detecção de padrões

---

## ⚙️ Como funciona

O processo de ML segue um fluxo padrão:

1. Coleta de dados  
2. Preparação dos dados  
3. Escolha do algoritmo  
4. Treinamento do modelo  
5. Avaliação  
6. Iteração (melhoria contínua)  
7. Inferência (uso em produção)

📌 Regra de ouro:
> **Garbage in, garbage out** → modelo é tão bom quanto os dados

---

## 🧠 Conceitos importantes

### 📊 Dados de treinamento

- Base usada para ensinar o modelo
- Etapa **mais crítica** do ML

📌 Problemas comuns:
- Dados incompletos
- Dados enviesados
- Dados inconsistentes

---

### 🏷️ Dados rotulados vs não rotulados

#### Dados rotulados
- Possuem **entrada + resposta correta (label)**
- Ex:
  - Imagem → "gato"
  - Email → "spam"
- Usado em **aprendizado supervisionado**

---

#### Dados não rotulados
- Apenas dados de entrada (sem resposta)
- Ex:
  - Imagens sem classificação
- Usado em **aprendizado não supervisionado**

---

### 🧱 Tipos de dados

#### 📋 Dados estruturados
- Organizados em tabelas (linhas e colunas)
- Ex:
  - Banco de dados
  - CSV
  - Planilhas
- Subtipos:
  - Dados tabulares
  - Séries temporais (ex: preços ao longo do tempo)

---

#### 🧩 Dados não estruturados
- Sem formato fixo
- Ex:
  - Texto
  - Imagens
  - Áudio
  - Vídeo
- Mais complexos de processar

---

### 🔍 Tipos de Machine Learning

#### 🟢 Supervisionado
- Usa **dados rotulados**
- Aprende relação: entrada → saída
- Ex:
  - Classificação
  - Regressão
- Objetivo: Prever resultados para novos dados

---

#### 🟡 Não supervisionado
- Usa **dados não rotulados**
- Ex:
  - Agrupamento (clustering)
  - Detecção de padrões
- Objetivo: Descobrir estrutura nos dados

---

#### 🔵 Reforço (Reinforcement Learning)
- Aprende por tentativa e erro
- Recebe:
  - Recompensa
  - Penalidade
- Ex:
  - Jogos
  - Robótica
- Aprende ao longo do tempo

---

#### 🟣 Semi-supervisionado
- Mistura:
  - Poucos dados rotulados
  - Muitos não rotulados
- Útil quando rotular é caro

---

### 🎯 Inferência

- Uso do modelo **já treinado**
- Faz previsões com novos dados

---

#### 📦 Inferência em lote (Batch)

- Processa grandes volumes de uma vez
- Ideal quando a velocidade do processo de tomada de decisão não é tão crucial quanto a precisão dos resultados
- Ex:
  - Relatórios
  - Análise de dados

---

#### ⚡ Inferência em tempo real

- Resposta imediata
- Baixa latência
- Ideal para aplicações em que a tomada de decisão imediata é fundamental
- Ex:
  - Chatbots
  - Recomendações
  - Detecção de fraude

---

## 💰 Modelo de cobrança (conceitual)

Não é direto no ML, mas na AWS:

- Treinamento → custo alto (compute intensivo)
- Inferência → custo contínuo (uso em produção)

📌 Otimização comum:
- Treinar pouco, inferir muito

---

## 🔒 Segurança (conceitual)

- Qualidade dos dados impacta segurança
- Riscos:
  - Vazamento de dados
  - Bias (viés)
  - Uso de dados sensíveis

---

## 🔁 Comparações importantes

---

### Dados rotulados vs não rotulados

| Rotulados | Não rotulados |
|----------|--------------|
| Possuem resposta | Não possuem |
| Mais caros | Mais baratos |
| Mais precisos | Mais exploratórios |

---

### Tipos de ML

| Tipo | Usa rótulo? | Objetivo |
|------|------------|----------|
| Supervisionado | Sim | Prever |
| Não supervisionado | Não | Descobrir padrões |
| Reforço | Não direto | Aprender com feedback |

---

### Inferência em lote vs tempo real

| Lote | Tempo real |
|-----|-----------|
| Alta latência | Baixa latência |
| Processa tudo de uma vez | Processa na hora |
| Mais barato | Mais caro |

---

## 🧠 Conceitos importantes para prova

- ML depende fortemente de **dados de qualidade**
- Dados rotulados → supervisionado
- Dados não rotulados → não supervisionado
- Inferência = uso do modelo treinado
- Treinamento ≠ inferência
- Dados estruturados vs não estruturados
- Batch vs real-time = **latência vs volume**

---

## ⚠️ Pegadinhas comuns

- Melhor algoritmo ≠ melhor resultado (dados são mais importantes)
- Mais dados ≠ melhor modelo (se dados forem ruins)
- Inferência não é treinamento
- Não supervisionado não significa "sem aprendizado"
- Tempo real ≠ sempre melhor (depende do caso)

---

## 🔁 Resumo rápido

- ML aprende padrões a partir de dados
- Processo: dados → treino → avaliação → inferência
- Tipos:
  - Supervisionado (com rótulo)
  - Não supervisionado (sem rótulo)
  - Reforço (feedback)
- Dados são o fator mais importante
- Inferência pode ser batch ou real-time

---

## 📌 Status de aprendizado

- [ ] Entendo o processo de ML
- [ ] Sei a diferença entre dados rotulados e não rotulados
- [ ] Sei diferenciar os tipos de ML
- [ ] Entendo inferência vs treinamento
- [ ] Sei quando usar batch vs tempo real
