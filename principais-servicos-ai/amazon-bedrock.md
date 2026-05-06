# 🪨 Amazon Bedrock

## 📌 O que é

O Amazon Bedrock é um serviço da **serverless** AWS que permite **usar modelos de IA generativa (Foundation Models) via API**, sem precisar treinar ou gerenciar infraestrutura.

📌 É a principal forma de trabalhar com **Generative AI na AWS**

---

## 🎯 Quando usar

- Quando quer usar **IA generativa pronta**
- Quando não quer treinar modelos do zero
- Quando precisa integrar IA rapidamente em aplicações

- Ex:
  - Chatbots
  - Geração de texto
  - Resumos automáticos
  - Geração de código
  - Análise de documentos com IA

---

## ⚙️ Como funciona

O Bedrock funciona como uma camada de abstração sobre modelos de IA:

1. Você escolhe um modelo (Foundation Model)  
2. Envia um prompt (entrada)  
3. Recebe uma resposta gerada  

📌 Tudo via API, sem gerenciar infraestrutura

---

## 🧠 Conceitos importantes

### 🧠 Modelos disponíveis (Model Providers)

- Bedrock oferece modelos de diferentes provedores

- Ex:
  - Anthropic (Claude)
  - AI21 Labs
  - Stability AI
  - Amazon (Titan)

📌 Você escolhe o modelo conforme o caso de uso

---

### 🧠 Agents for Bedrock

- Permite criar agentes que executam tarefas automaticamente
- Podem:
  - Consultar APIs
  - Tomar decisões
  - Executar fluxos

📌 Usado para automação com IA

---

### 🔐 Guardrails

- Controles de segurança e governança
- Permite:
  - Filtrar conteúdo
  - Evitar respostas inadequadas
  - Definir limites

📌 Importante para produção

---

## 💰 Modelo de cobrança

- Baseado em:
  - Tokens de entrada (input)
  - Tokens de saída (output)

📌 Mais uso → maior custo

---

## 🔒 Segurança

- Integra com:
  - IAM (controle de acesso)
  - VPC (isolamento)
- Dados não são usados para treinar modelos por padrão

📌 Foco em privacidade e controle

---

## 🔁 Comparações importantes

---

### Bedrock vs SageMaker

| Bedrock | SageMaker |
|--------|----------|
| Usa modelos prontos | Cria e treina modelos |
| Sem infraestrutura | Gerencia infraestrutura |
| Mais simples | Mais complexo |
| Rápido para começar | Mais flexível |

---

### Bedrock vs AI Services (Rekognition, Comprehend, etc)

| Bedrock | AI Services |
|--------|-------------|
| Generative AI | IA tradicional |
| Mais flexível | Mais específico |
| Baseado em prompts | Baseado em APIs fixas |

---

### RAG vs Fine-tuning

| RAG | Fine-tuning |
|-----|------------|
| Usa dados externos | Treina o modelo |
| Mais barato | Mais caro |
| Atualização fácil | Atualização difícil |

---

## 🧠 Conceitos importantes para prova

- Bedrock = **Generative AI como serviço**
- Usa Foundation Models
- Não precisa treinar modelo
- Prompt é essencial
- RAG é alternativa ao fine-tuning
- Suporta múltiplos provedores
- Guardrails = segurança

---

## ⚠️ Pegadinhas comuns

- Bedrock não treina modelos do zero
- Não precisa gerenciar infraestrutura
- Não é limitado a um único modelo
- RAG não altera o modelo
- Fine-tuning não é sempre necessário

---

## 🔁 Resumo rápido

- Bedrock = usar IA generativa via API
- Baseado em Foundation Models
- Entrada = prompt
- Saída = conteúdo gerado
- Suporta:
  - RAG
  - Fine-tuning
- Foco em simplicidade e integração

---

## 📌 Status de aprendizado

- [ ] Entendo o que é o Bedrock
- [ ] Sei quando usar vs SageMaker
- [ ] Entendo o papel dos Foundation Models
- [ ] Sei o que é RAG vs Fine-tuning
- [ ] Entendo como prompts influenciam resultados
