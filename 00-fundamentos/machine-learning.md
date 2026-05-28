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

## 🧪 Técnicas e casos de uso de ML
<img width="931" height="221" alt="image" src="https://github.com/user-attachments/assets/0badbf7d-2d7e-49d0-96a1-fb8658ddcd81" />

### 🟢 Aprendizado supervisionado (Supervised Learning)
<img width="849" height="420" alt="image" src="https://github.com/user-attachments/assets/f4867291-31fa-4d14-b0d5-12a250f57b76" />

- Usa dados rotulados
- Aprende:
  - Entrada → saída
- Objetivo:
  - Fazer previsões

📌 Subcategorias:
- Classificação
- Regressão

---

#### 🏷️ Classificação (Classification)

- Prevê categorias/classes

- Ex:
  - Spam vs não spam
  - Fraude vs legítimo
  - Diagnóstico médico

📌 Casos de uso:
- Detecção de fraudes
- Classificação de imagens
- Retenção de clientes

---

#### 📈 Regressão (Regression)

- Prevê valores numéricos contínuos

- Ex:
  - Preço de imóveis
  - Temperatura
  - Crescimento populacional

📌 Casos de uso:
- Previsão do tempo
- Mercado financeiro
- Popularidade de anúncios

---

### 🟡 Aprendizado não supervisionado (Unsupervised Learning)
<img width="444" height="541" alt="image" src="https://github.com/user-attachments/assets/ab023048-9a2a-44b6-919f-4285c4f7ccc4" />

- Usa dados não rotulados
- Descobre:
  - Padrões
  - Estruturas
  - Relacionamentos

📌 Subcategorias:
- Clustering
- Redução de dimensionalidade

---

#### 🧩 Agrupamento em clusters (Clustering)

- Agrupa dados semelhantes

- Ex:
  - Segmentação de clientes
  - Marketing direcionado
  - Sistemas de recomendação

📌 Objetivo:
- Encontrar grupos naturalmente

---

#### 📉 Redução de dimensionalidade (Dimensionality Reduction)

- Reduz quantidade de atributos/dimensões
- Mantém informações importantes

📌 Casos de uso:
- Visualização de dados
- Compressão
- Descoberta de padrões

---

### 🔵 Aprendizado por reforço (Reinforcement Learning)

- Aprende por tentativa e erro
- Recebe:
  - Recompensas
  - Penalidades

📌 Componentes:
- Agente
- Ambiente
- Ações
- Recompensas

---

#### 🏎️ Exemplo: AWS DeepRacer
<img width="509" height="395" alt="image" src="https://github.com/user-attachments/assets/50a2cba9-4a5b-4fc7-9f36-5a69fe51eb89" />

- Agente:
  - Carro virtual

- Ambiente:
  - Pista virtual

- Objetivo:
  - Completar pista rapidamente sem sair dela

📌 Aprende continuamente com feedback

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

### Classificação vs Regressão

| Classificação | Regressão |
|--------------|-----------|
| Prevê categorias | Prevê números |
| Spam/não spam | Preço de casa |
| Resultado discreto | Resultado contínuo |

---

### Clustering vs Classificação

| Clustering | Classificação |
|------------|--------------|
| Não supervisionado | Supervisionado |
| Sem rótulos | Com rótulos |
| Descobre grupos | Prevê categorias |

---

## 🧠 Conceitos importantes para prova

- ML depende fortemente de **dados de qualidade**
- Dados rotulados → supervisionado
- Dados não rotulados → não supervisionado
- Inferência = uso do modelo treinado
- Treinamento ≠ inferência
- Dados estruturados vs não estruturados
- Batch vs real-time = **latência vs volume**
- Supervisionado usa dados rotulados
- Não supervisionado usa dados não rotulados
- Classificação → categorias
- Regressão → valores numéricos
- Clustering → agrupamento
- Reinforcement learning → tentativa e erro

---

## ⚠️ Pegadinhas comuns

- Melhor algoritmo ≠ melhor resultado (dados são mais importantes)
- Mais dados ≠ melhor modelo (se dados forem ruins)
- Inferência não é treinamento
- Não supervisionado não significa "sem aprendizado"
- Tempo real ≠ sempre melhor (depende do caso)
- Classificação ≠ regressão
- Clustering não usa rótulos
- Reinforcement learning não aprende com dataset rotulado tradicional
- Redução de dimensionalidade não significa perda total de informação

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
