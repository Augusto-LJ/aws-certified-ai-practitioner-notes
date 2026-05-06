# 🧠 Amazon SageMaker

## 📌 O que é

O Amazon SageMaker é um serviço da AWS que permite **construir, treinar e implantar modelos de Machine Learning em escala**.

📌 É uma plataforma completa (end-to-end) para ML:
- Preparação de dados
- Treinamento
- Deploy (inferência)

---

## 🎯 Quando usar

- Quando você precisa **criar e treinar modelos próprios**
- Quando quer **controle sobre o processo de ML**
- Para workloads mais customizados

- Ex:
  - Treinar modelos com dados próprios
  - Criar pipelines de ML
  - Deploy de modelos personalizados
  - Experimentação com algoritmos

---

## ⚙️ Como funciona

O SageMaker cobre todo o ciclo de vida de ML:

1. Preparação de dados  
2. Construção do modelo  
3. Treinamento  
4. Avaliação  
5. Deploy (endpoint)  
6. Inferência  

📌 Pode usar:
- Código próprio
- Modelos prontos
- Frameworks (TensorFlow, PyTorch)

---

## 🧠 Conceitos importantes

### 🧪 SageMaker Studio

- IDE baseada na web para ML
- Interface central para:
  - Treinamento
  - Debug
  - Deploy

📌 Ambiente visual para desenvolvimento

---

### 🏗️ Treinamento (Training Jobs)

- Processo de treinar modelos com dados
- Executado em instâncias gerenciadas

- Ex:
  - Treinar modelo de classificação
  - Treinar modelo de previsão

📌 Você define:
- Dados
- Algoritmo
- Recursos computacionais

---

### 📦 Modelos (Models)

- Artefato treinado pronto para uso
- Pode ser:
  - Criado por você
  - Importado

---

### 🚀 Deploy / Endpoint (Inference Endpoint)

- Publica o modelo como API
- Permite inferência em tempo real

📌 Endpoint = ponto de acesso ao modelo

---

### 📦 Batch Transform (Inferência em lote)

- Processa grandes volumes de dados
- Sem necessidade de endpoint ativo

- Ex:
  - Processamento de arquivos
  - Análises periódicas

---

### ⚡ Real-time Inference

- Inferência em tempo real
- Baixa latência

- Ex:
  - Recomendação
  - Fraude
  - APIs

---

### 🤖 SageMaker JumpStart

- Biblioteca de modelos e soluções prontas
- Inclui:
  - Foundation Models
  - Templates

📌 Acelera desenvolvimento

---

### 🔗 Pipelines (SageMaker Pipelines)

- Automatiza fluxo de ML
- Define etapas como:
  - Treinamento
  - Validação
  - Deploy

📌 CI/CD para Machine Learning

---

### 🏷️ Data Labeling (Ground Truth)

- Serviço de rotulagem de dados
- Pode usar:
  - Humanos
  - Automação

📌 Importante para aprendizado supervisionado

---

## 💰 Modelo de cobrança

- Baseado em uso de recursos:
  - Instâncias de treinamento
  - Instâncias de inferência
  - Armazenamento

📌 Quanto mais processamento → maior custo

---

## 🔒 Segurança

- Integra com:
  - IAM (controle de acesso)
  - VPC (isolamento de rede)
- Proteção de dados durante:
  - Treinamento
  - Inferência

---

## 🔁 Comparações importantes

---

### SageMaker vs Bedrock

| SageMaker | Bedrock |
|----------|--------|
| Cria e treina modelos | Usa modelos prontos (Foundation Models) |
| Alto controle | Baixo controle |
| Mais complexo | Mais simples |
| Mais flexível | Mais rápido de usar |

---

### SageMaker vs AI Services (Rekognition, Comprehend, etc)

| SageMaker | AI Services |
|----------|-------------|
| Customização total | Pronto para uso |
| Precisa treinar | Não precisa treinar |
| Mais complexo | Mais simples |

---

### Batch vs Real-time no SageMaker

| Batch Transform | Real-time Endpoint |
|---------------|-------------------|
| Sem endpoint ativo | Endpoint ativo |
| Mais barato | Mais caro |
| Alta latência | Baixa latência |

---

## 🧠 Conceitos importantes para prova

- SageMaker = **plataforma completa de ML**
- Usado para:
  - Treinar modelos
  - Customizar modelos
- Endpoint = inferência em tempo real
- Batch Transform = inferência em lote
- JumpStart = modelos prontos
- Pipelines = automação

---

## ⚠️ Pegadinhas comuns

- SageMaker ≠ serviço pronto (exige configuração)
- Não é serverless por padrão
- Mais complexo que Bedrock
- Precisa gerenciar recursos (instâncias)
- Endpoint ativo gera custo contínuo

---

## 🔁 Resumo rápido

- SageMaker = construir, treinar e deploy de ML
- Alto controle e flexibilidade
- Suporta:
  - Treinamento
  - Batch
  - Real-time
- Integra com todo ecossistema AWS

---

## 📌 Status de aprendizado

- [ ] Entendo o que é o SageMaker
- [ ] Sei quando usar vs Bedrock
- [ ] Entendo treinamento vs inferência no SageMaker
- [ ] Sei o que é endpoint
- [ ] Entendo Batch vs Real-time
