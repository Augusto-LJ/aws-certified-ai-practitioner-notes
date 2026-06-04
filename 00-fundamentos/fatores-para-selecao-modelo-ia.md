# 🎯 Seleção de Modelos de IA Generativa

## 📌 O que é

Ao utilizar IA generativa, é importante escolher o modelo mais adequado para o caso de uso.

📌 Não existe um modelo melhor para tudo.

Cada modelo possui:
- Capacidades diferentes
- Custos diferentes
- Requisitos diferentes
- Casos de uso específicos

---

## 🎯 Quando analisar

Sempre que for necessário:

- Criar uma aplicação com IA generativa
- Escolher um Foundation Model (FM)
- Comparar modelos disponíveis no Amazon Bedrock
- Avaliar custo vs desempenho

---

## ⚙️ Principais fatores de decisão

### 🧠 Tipo de modelo (Model Type)

O primeiro passo é identificar a tarefa que será executada.

- Ex:
  - Geração de texto
  - Geração de imagens
  - Chatbots
  - Tradução
  - Resumo
  - Geração de código

📌 Alguns modelos são especializados em determinadas tarefas.

---

### 🚀 Requisitos de desempenho (Performance Requirements)

Avalie:

- Acurácia (Accuracy)
- Confiabilidade (Reliability)
- Consistência das respostas
- Latência (Latency)

📌 O modelo deve atender aos requisitos do negócio.

---

### ⚙️ Capacidades (Capabilities)

Cada modelo possui capacidades diferentes.

- Ex:
  - Texto
  - Código
  - Imagem
  - Embeddings
  - Busca semântica
  - Multimodalidade

📌 Nem todo modelo suporta todas as funcionalidades.

---

### 🏗️ Restrições (Constraints)

Considere limitações relacionadas a:

- CPU
- GPU
- Memória
- Dados disponíveis
- Ambiente de implantação

- Ex:
  - Cloud
  - On-premises

📌 Alguns modelos exigem muito mais recursos computacionais.

---

### ⚖️ Conformidade (Compliance)

Avalie requisitos relacionados a:

- Privacidade
- Segurança
- Regulamentações
- Governança

Também considere riscos como:

- Bias
- Toxicity
- Hallucinations

📌 Especialmente importante em:
- Saúde
- Finanças
- Jurídico

---

### 💰 Custo (Cost)

Avalie:

- Implantação
- Inferência
- Treinamento
- Armazenamento
- Hardware

📌 Regra geral:

| Modelos maiores | Modelos menores |
|----------------|----------------|
| Mais precisos | Menos precisos |
| Mais caros | Mais baratos |
| Mais lentos | Mais rápidos |
| Menos opções de implantação | Mais flexíveis |

---

## 🏢 Exemplos de Foundation Models

### 🤖 Amazon Titan

#### Capacidades

- Resumo
- Classificação
- Perguntas e respostas
- Embeddings
- Busca semântica

#### Casos de uso

- Atendimento ao cliente
- Pesquisa corporativa
- Aplicações de busca

---

### 🧠 Claude (Anthropic)

#### Capacidades

- Geração de conteúdo
- Resumo
- Tradução
- Perguntas e respostas
- Geração de código

#### Casos de uso

- Assistentes virtuais
- Desenvolvimento de software
- Análise de documentos

---

### 🦙 Llama (Meta)

#### Capacidades

- Chat
- Resumo
- Análise de sentimento
- Geração de texto

#### Casos de uso

- Chatbots
- Atendimento ao cliente

---

### ✍️ Command (Cohere)

#### Capacidades

- Geração de texto
- Perguntas e respostas
- Resumo
- Extração de informações

#### Casos de uso

- Atendimento ao cliente
- Descrições de produtos

---

### 🎨 Stable Diffusion (Stability AI)

#### Capacidades

- Geração de imagens
- Edição de imagens
- Aprimoramento visual

#### Casos de uso

- Marketing
- Publicidade
- Jogos
- Design

---

### 📚 Jurassic-2 (AI21 Labs)

#### Capacidades

- Geração de texto
- Resumo
- Parafraseamento
- Chat

#### Casos de uso

- Documentação
- Resumos corporativos

---

## 🔁 Comparações importantes

### Claude vs Llama

| Claude | Llama |
|----------|----------|
| Forte em análise e geração de conteúdo | Forte em conversação |
| Muito usado para documentos | Muito usado para chatbots |

---

### Titan vs Claude

| Titan | Claude |
|--------|---------|
| Modelo da AWS | Modelo da Anthropic |
| Possui embeddings | Forte em geração de texto e código |

---

### Texto vs Imagem

| Modelos de texto | Modelos de imagem |
|-----------------|------------------|
| Claude | Stable Diffusion |
| Titan Text | Stable Diffusion |
| Llama | Stable Diffusion |

---

## 🧠 Conceitos importantes para prova

- Não existe um único modelo ideal
- A escolha depende do caso de uso
- Avaliar:
  - Capacidades
  - Custo
  - Desempenho
  - Restrições
  - Conformidade
- Foundation Models possuem características diferentes
- Amazon Bedrock permite acesso a múltiplos modelos através de uma única API

---

## ⚠️ Pegadinhas comuns

- Modelo maior não significa melhor para todos os cenários
- Modelo mais caro não significa melhor custo-benefício
- Nem todo modelo gera imagens
- Nem todo modelo gera código
- A escolha do modelo depende dos requisitos da aplicação

---

## 🔁 Resumo rápido

- Escolha o modelo com base no caso de uso
- Considere:
  - Tipo de tarefa
  - Desempenho
  - Capacidades
  - Restrições
  - Conformidade
  - Custo
- Amazon Bedrock oferece diversos Foundation Models
- Diferentes modelos são otimizados para diferentes tarefas

---

## 📌 Status de aprendizado

- [ ] Sei quais fatores analisar ao escolher um modelo
- [ ] Entendo a diferença entre capacidades e desempenho
- [ ] Sei quando considerar conformidade
- [ ] Entendo o impacto do custo na escolha do modelo
- [ ] Conheço os principais Foundation Models disponíveis no Bedrock
