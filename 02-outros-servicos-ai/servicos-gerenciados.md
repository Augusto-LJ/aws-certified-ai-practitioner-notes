# 🧠 AI Services Gerenciados (Managed AI Services)

## 📌 O que é

AI Services Gerenciados (Managed AI Services) são serviços da AWS que utilizam Machine Learning **pré-treinado**, permitindo adicionar inteligência às aplicações **sem precisar treinar modelos**.

📌 Características:
- Prontos para uso (out-of-the-box)
- Baseados em API
- Não exigem conhecimento profundo de ML

---

## 🎯 Quando usar

- Quando você **não quer treinar modelos**
- Quando precisa de **solução rápida**
- Quando o problema já é comum e bem definido

- Ex:
  - Analisar texto (sentimento, entidades)
  - Extrair texto de documentos
  - Converter fala em texto
  - Criar chatbot básico
  - Analisar imagens

---

## ⚙️ Como funciona

Fluxo padrão:

1. Aplicação envia dados (texto, imagem, áudio)
2. Serviço processa usando modelos pré-treinados
3. Retorna resultado via API

📌 Você só consome → não treina

---

## 🧠 Conceitos importantes

### ⚡ Serviços prontos (Pre-trained Models)

- Modelos já treinados pela AWS
- Não precisam de treinamento adicional
- Funcionam para casos comuns

📌 Foco em produtividade

---

### 🔌 Integração via API

- Todos os serviços são acessados via API
- Fácil integração com aplicações

📌 Ideal para backend e automação

---

### 🧱 Sem necessidade de treinamento

- Diferente do SageMaker
- Apenas envia dados e recebe resposta

📌 Menor complexidade

---

## 📦 Serviços

---

### 📝 Amazon Comprehend (NLP - Natural Language Processing)

- Analisa texto automaticamente
- Detecta:
  - Sentimento
  - Entidades
  - Linguagem
  - Tópicos

- Ex:
  - Classificar feedback de clientes
  - Identificar nomes, lugares, datas

---

### 🌍 Amazon Translate

- Tradução automática de texto

- Ex:
  - Traduzir conteúdo de aplicações
  - Suporte multilíngue

---

### 📄 Amazon Textract (OCR - Optical Character Recognition)

- Extrai texto de documentos

- Ex:
  - PDFs
  - Imagens escaneadas
- Também extrai:
  - Tabelas
  - Formulários

---

### 💬 Amazon Lex

- Criação de chatbots com NLP

- Ex:
  - Assistentes virtuais
  - Bots de atendimento

📌 Base do Alexa

---

### 🔊 Amazon Polly (Text-to-Speech)

- Converte texto em áudio

- Ex:
  - Leitura de textos
  - Acessibilidade

---

### 🎙️ Amazon Transcribe (Speech-to-Text)

- Converte áudio em texto

- Ex:
  - Transcrição de chamadas
  - Legendas automáticas

---

### 👁️ Amazon Rekognition

- Análise de imagens e vídeos

- Detecta:
  - Objetos
  - Pessoas
  - Rostos
  - Emoções

- Ex:
  - Moderação de conteúdo
  - Reconhecimento facial

---

## 💰 Modelo de cobrança

- Baseado em uso:
  - Número de requisições
  - Volume de dados processados

📌 Ex:
- Texto analisado
- Minutos de áudio
- Imagens processadas

---

## 🔒 Segurança

- Integração com:
  - IAM (controle de acesso)
- Processamento gerenciado pela AWS

📌 Responsabilidade:
- Você → dados enviados
- AWS → modelo e processamento

---

## 🔁 Comparações importantes

---

### AI Services vs SageMaker

| AI Services | SageMaker |
|------------|----------|
| Pronto para uso | Precisa treinar |
| Sem ML avançado | ML completo |
| Rápido | Mais complexo |

---

### AI Services vs Bedrock

| AI Services | Bedrock |
|------------|--------|
| Tarefas específicas | Generative AI |
| Modelos fixos | Foundation Models |
| Menos flexível | Mais flexível |

---

### Serviços (quando usar cada um)

| Serviço | Uso principal |
|--------|-------------|
| Comprehend | Análise de texto |
| Translate | Tradução |
| Textract | OCR (extrair texto de docs) |
| Lex | Chatbot |
| Polly | Texto → áudio |
| Transcribe | Áudio → texto |
| Rekognition | Imagem/vídeo |

---

## 🧠 Conceitos importantes para prova

- AI Services = **sem necessidade de treinamento**
- Baseados em API
- Resolvem problemas comuns
- Escolha depende do tipo de dado:
  - Texto → Comprehend
  - Áudio → Transcribe
  - Imagem → Rekognition
  - Documento → Textract

---

## ⚠️ Pegadinhas comuns

- AI Services ≠ Generative AI
- Não precisam de treinamento
- Lex não é LLM (é chatbot baseado em NLP)
- Textract ≠ Comprehend (documento vs texto)
- Polly ≠ Transcribe (direções opostas)

---

## 🔁 Resumo rápido

- Serviços prontos de IA da AWS
- Sem necessidade de treinar modelos
- Baseados em API
- Cada serviço resolve um tipo específico de problema
- Ideais para desenvolvimento rápido

---

## 📌 Status de aprendizado

- [ ] Sei o que são AI Services
- [ ] Sei quando usar vs SageMaker
- [ ] Sei quando usar vs Bedrock
- [ ] Sei diferenciar os principais serviços
- [ ] Consigo escolher o serviço correto para cada cenário
