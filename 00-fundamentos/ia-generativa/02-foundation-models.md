# 🧱 Foundation Models (Modelos Fundamentais)

## 📌 O que são

Foundation Models (FMs), ou **Modelos Fundamentais**, são modelos de IA treinados em **grandes volumes de dados** capazes de realizar diversas tarefas sem terem sido criados para apenas uma aplicação específica.

Eles são a base da IA Generativa moderna e podem ser adaptados para diferentes cenários.

<img width="906" height="367" alt="image" src="https://github.com/user-attachments/assets/bba00897-4f12-43aa-8aaf-fa0e66907f73" />

Exemplos de tarefas:

- Geração de texto
- Tradução
- Resumos
- Geração de código
- Criação de imagens
- Resposta a perguntas

📌 Diferentemente dos modelos tradicionais de Machine Learning, um Foundation Model pode ser reutilizado em diversos domínios e aplicações.

---

## 🎯 Por que eles são importantes?

Antes dos Foundation Models, normalmente era necessário criar um modelo diferente para cada problema.

Exemplo:

- Um modelo para classificação de imagens
- Outro para tradução
- Outro para geração de texto

Com Foundation Models:

- Um único modelo pode atender diversos casos de uso.
- Basta adaptá-lo para a necessidade da aplicação.

Isso reduziu drasticamente o custo e o tempo para desenvolver soluções de IA.

---

## ⚙️ Como funcionam

Em alto nível, o processo ocorre da seguinte forma:

```text
Grandes volumes de dados
            ↓
     Pré-treinamento
            ↓
     Foundation Model
            ↓
 Personalização (Prompt, RAG,
 Fine-tuning, etc.)
            ↓
      Aplicação final
```

O modelo aprende padrões gerais presentes nos dados durante o treinamento.

Posteriormente, ele pode ser utilizado diretamente ou adaptado para tarefas específicas.

---

# 🔄 Ciclo de Vida dos Foundation Models

Os Foundation Models passam por diversas etapas até serem utilizados em aplicações reais.

---

## 📥 1. Seleção de dados (Data Selection)

Nesta etapa são coletados grandes volumes de dados para treinamento.

Os dados podem incluir:

- Texto
- Código
- Imagens
- Áudio
- Vídeos

A qualidade desses dados é extremamente importante.

📌 Garbage In, Garbage Out

Dados ruins produzem modelos ruins.

---

## 🧠 2. Pré-treinamento (Pre-training)

É o treinamento inicial do modelo em larga escala.

Normalmente utiliza **aprendizado autossupervisionado (Self-supervised Learning)**, onde o próprio conjunto de dados fornece os "rótulos" utilizados durante o treinamento.

Durante essa etapa o modelo aprende:

- Linguagem
- Contexto
- Relações entre palavras
- Conhecimento geral
- Padrões estatísticos

Características:

- Alto custo computacional
- Pode levar semanas ou meses
- Exige enorme quantidade de dados

📌 É a etapa mais cara de todo o processo.

---

## 🔄 Pré-treinamento contínuo (Continual Pre-training)

Após o treinamento inicial, um Foundation Model pode continuar sendo treinado com novos dados.

Objetivos:

- Expandir seu conhecimento
- Melhorar desempenho
- Aprender novos domínios

Sem precisar reiniciar todo o treinamento do zero.

---

## ⚙️ 3. Otimização (Optimization)

Após o pré-treinamento, o modelo pode ser adaptado para casos específicos.

As principais técnicas são:

- Fine-tuning
- Prompt Engineering
- RAG (Retrieval-Augmented Generation)
- Ajuste de parâmetros de inferência
- RLHF (Reinforcement Learning from Human Feedback)

📌 O objetivo é tornar o modelo mais útil para aplicações reais.

---

## 📊 4. Avaliação (Evaluation)

Antes de colocar um modelo em produção, é necessário avaliar sua qualidade.

Alguns critérios:

- Precisão
- Qualidade das respostas
- Segurança
- Viés (Bias)
- Toxicidade
- Desempenho

A AWS oferece ferramentas para avaliação de modelos no Amazon Bedrock.

---

## 🚀 5. Implantação (Deployment)

Após aprovado, o modelo pode ser disponibilizado para uso.

Exemplos:

- APIs
- Chatbots
- Sistemas internos
- Aplicações Web
- Assistentes inteligentes

É nesta etapa que o modelo começa a gerar valor para o negócio.

---

## 🔁 6. Feedback e melhoria contínua

Depois da implantação, o modelo continua sendo monitorado.

As melhorias podem envolver:

- Feedback dos usuários
- Novos dados
- Ajustes de prompts
- Novo Fine-tuning
- Atualizações do modelo

Esse processo é contínuo.

---

# 🎯 Como adaptar um Foundation Model

Existem várias formas de adaptar um Foundation Model para uma aplicação.

As principais são:

- Prompt Engineering
- RAG
- Fine-tuning

Cada técnica possui vantagens e casos de uso específicos.

📌 Na certificação AI Practitioner, saber diferenciar **RAG** e **Fine-tuning** é muito importante.

---

# ☁️ Foundation Models no Amazon Bedrock

O Amazon Bedrock fornece acesso a diversos Foundation Models através de uma API única.

Eles podem ser utilizados sem necessidade de:

- Treinar modelos
- Gerenciar infraestrutura
- Implantar servidores

Alguns provedores disponíveis:

- Amazon
  - Nova
  - Titan
- Anthropic (Claude)
- Meta
- Cohere
- AI21 Labs
- Stability AI

📌 O Bedrock abstrai toda a infraestrutura necessária para utilizar esses modelos.

---

# 🔁 Comparação importante

## Foundation Model vs Modelo tradicional de Machine Learning

| Foundation Model | Modelo tradicional |
|------------------|--------------------|
| Treinado em grandes volumes de dados | Treinado para uma tarefa específica |
| Reutilizável | Especializado |
| Muito flexível | Pouco flexível |
| Base da IA Generativa | Base do ML tradicional |

---

# 🧠 Conceitos importantes para prova

- Foundation Models são treinados em grandes volumes de dados.
- Não são criados para apenas uma tarefa.
- Podem ser adaptados para vários casos de uso.
- São a base da IA Generativa moderna.
- Podem ser personalizados usando:
  - Prompt Engineering
  - RAG
  - Fine-tuning
- O Amazon Bedrock fornece acesso a vários Foundation Models.

---

# ⚠️ Pegadinhas comuns

- Foundation Models **não** são treinados para apenas uma tarefa.
- Um Foundation Model **não precisa** ser retreinado para cada aplicação.
- Prompt Engineering e RAG **não alteram** os pesos do modelo.
- Fine-tuning altera o comportamento do modelo por meio de treinamento adicional.
- Foundation Model **não é sinônimo de LLM**.

> **LLMs (Large Language Models)** são um tipo de Foundation Model voltado para linguagem natural. Também existem Foundation Models para imagens, áudio, vídeo e embeddings.

---

# 🔁 Resumo rápido

- Foundation Models são modelos de IA de propósito geral.
- São treinados em grandes volumes de dados.
- Servem de base para aplicações de IA Generativa.
- Passam pelas etapas:
  - Seleção de dados
  - Pré-treinamento
  - Otimização
  - Avaliação
  - Implantação
  - Melhoria contínua
- Podem ser adaptados usando Prompt Engineering, RAG ou Fine-tuning.

---

# 📌 Status de aprendizado

- [ ] Entendo o que são Foundation Models
- [ ] Sei por que eles revolucionaram a IA Generativa
- [ ] Conheço o ciclo de vida de um Foundation Model
- [ ] Entendo a diferença entre Foundation Model e ML tradicional
- [ ] Sei como Foundation Models são utilizados no Amazon Bedrock
