# 🏗️ Visão técnica do Amazon Bedrock

Esta página aborda a arquitetura, integrações e principais considerações técnicas do Amazon Bedrock.

O foco é entender **como o serviço funciona nos bastidores** e **como ele se integra ao ecossistema AWS**.

---

# 🏛️ Arquitetura do Amazon Bedrock

O Amazon Bedrock é um serviço **totalmente gerenciado e serverless** que fornece acesso a **Foundation Models (FMs)** por meio de uma API unificada.

Uma arquitetura típica envolve:

1. Usuário envia um prompt.
2. A aplicação processa a solicitação.
3. O Bedrock recupera informações (quando utiliza RAG).
4. O modelo gera uma resposta.
5. A resposta é devolvida ao usuário.

---

## 🔄 Fluxo da arquitetura

<img width="1008" height="537" alt="image" src="https://github.com/user-attachments/assets/af117577-9cb2-45bb-8c78-f8410e78ee47" />

### 1️⃣ Consulta do usuário

O usuário envia uma pergunta em linguagem natural por meio de uma aplicação.

Exemplos:

- Chatbot
- Aplicação web
- Amazon Lex

---

### 2️⃣ Camada de processamento

A aplicação processa a solicitação.

Normalmente utiliza:

- AWS Lambda
- APIs
- Lógica de negócio

Essa camada é responsável por:

- Validar a requisição
- Orquestrar chamadas
- Integrar outros serviços

---

### 3️⃣ Dados empresariais

Os documentos da empresa ficam armazenados, normalmente, no:

- Amazon S3

Esses documentos podem conter:

- Manuais
- Políticas internas
- Contratos
- Catálogos
- Documentação

---

### 4️⃣ Knowledge Bases for Amazon Bedrock

As **Knowledge Bases** sincronizam e indexam os documentos corporativos.

São utilizadas para implementar **RAG (Retrieval-Augmented Generation)**.

Durante uma consulta:

1. O Bedrock procura documentos relevantes.
2. Recupera o contexto.
3. Envia esse contexto ao modelo.
4. O modelo gera uma resposta mais precisa.

📌 O modelo passa a responder utilizando conhecimento da empresa.

---

### 5️⃣ Geração da resposta

O Foundation Model gera a resposta utilizando:

- Prompt do usuário
- Contexto recuperado (RAG)
- Configurações da aplicação

---

### 6️⃣ Resposta ao usuário

A resposta é enviada para a aplicação e apresentada ao usuário em linguagem natural.

---

# 🔌 Integrações do Amazon Bedrock

O Amazon Bedrock integra-se facilmente com diversos serviços da AWS.

---

## 🧠 Amazon SageMaker AI

Utilizado quando é necessário trabalhar com modelos personalizados.

Enquanto o Bedrock fornece **Foundation Models prontos**, o SageMaker permite:

- Treinar modelos
- Ajustar modelos personalizados
- Preparar dados

📌 Bedrock e SageMaker podem ser utilizados juntos.

---

## 🔎 Amazon Kendra

O Amazon Kendra fornece **pesquisa empresarial inteligente**.

Quando integrado ao Bedrock:

- realiza pesquisa semântica;
- recupera documentos relevantes;
- melhora aplicações baseadas em RAG.

📌 Muito utilizado para chatbots corporativos.

---

## ⚙️ AWS Lambda

Responsável por executar a lógica da aplicação.

Pode ser utilizado para:

- Chamar o Bedrock
- Processar prompts
- Formatar respostas
- Integrar outros serviços

📌 É a integração mais comum.

---

## 🪣 Amazon S3

Armazena documentos utilizados pela aplicação.

Exemplos:

- PDFs
- Word
- Planilhas
- Base documental

Esses documentos podem alimentar:

- Knowledge Bases
- Fine-tuning
- Aplicações RAG

---

## 🔍 Amazon OpenSearch Service

Muito utilizado junto com RAG.

Responsável por:

- Indexar documentos
- Pesquisa semântica
- Recuperação rápida de informações

📌 Frequentemente utilizado como banco vetorial em soluções RAG.

---

## 🔐 AWS IAM

Controla quem pode acessar:

- Modelos
- APIs
- Bases de conhecimento
- Recursos do Bedrock

Segue o princípio do **menor privilégio (Least Privilege)**.

---

## 📊 Amazon CloudWatch

Monitora aplicações que utilizam Bedrock.

Permite acompanhar:

- Tempo de resposta
- Erros
- Uso da API
- Desempenho

Também pode gerar alarmes automaticamente.

---

## 📅 Amazon EventBridge

Permite criar arquiteturas orientadas a eventos.

Exemplo:

1. Novo arquivo enviado ao S3.
2. EventBridge detecta o evento.
3. Lambda é executado.
4. Bedrock cria automaticamente um resumo do documento.

📌 Muito usado para automações.

---

# ⚙️ Considerações de integração

Ao integrar o Bedrock com outros serviços, alguns fatores devem ser considerados.

---

## 🔐 Segurança e conformidade

Garanta:

- Criptografia dos dados
- Controle de acesso (IAM)
- Conformidade regulatória
- Proteção das informações

📌 Segurança é prioridade em aplicações corporativas.

---

## ⚡ Otimização de desempenho

Escolha o modelo adequado para cada caso de uso.

Considere:

- Latência
- Precisão
- Custo
- Quantidade de tokens

📌 Modelos maiores nem sempre são a melhor escolha.

---

## 📈 Planejamento de escalabilidade

Projete a aplicação para suportar crescimento.

Considere:

- Número de usuários simultâneos
- Tempo de resposta
- Volume de requisições
- Consumo de recursos

Como o Bedrock é **serverless**, o escalonamento é automático, mas a arquitetura da aplicação também deve acompanhar esse crescimento.

---

# 🔁 Comparações importantes

---

### Amazon Bedrock vs Amazon SageMaker

| Amazon Bedrock | Amazon SageMaker |
|----------------|------------------|
| Usa Foundation Models prontos | Treina e gerencia modelos personalizados |
| Serverless | Ambiente completo de Machine Learning |
| API unificada | Controle total do ciclo de vida do modelo |
| Ideal para IA Generativa | Ideal para Machine Learning tradicional |

---

### Knowledge Base vs Amazon OpenSearch

| Knowledge Base | OpenSearch |
|----------------|-----------|
| Recurso do Bedrock | Serviço AWS independente |
| Gerencia documentos para RAG | Indexa e pesquisa documentos |
| Simplifica aplicações RAG | Fornece pesquisa semântica eficiente |

---

### Lambda vs EventBridge

| Lambda | EventBridge |
|---------|------------|
| Executa código | Dispara eventos |
| Processa lógica | Orquestra eventos |
| Integra serviços | Automatiza fluxos |

---

# 🧠 Conceitos importantes para prova

- O Amazon Bedrock é um serviço **serverless**.
- Knowledge Bases implementam **RAG** de forma gerenciada.
- O Amazon S3 é uma fonte comum de documentos para RAG.
- O AWS Lambda normalmente orquestra chamadas ao Bedrock.
- O Amazon Kendra adiciona pesquisa empresarial inteligente.
- O OpenSearch melhora a recuperação de documentos.
- O CloudWatch monitora aplicações do Bedrock.
- O EventBridge automatiza fluxos baseados em eventos.
- O IAM controla permissões de acesso.
- Segurança e conformidade são responsabilidades importantes na integração.

---

# ⚠️ Pegadinhas comuns

- Knowledge Base **não substitui** o Amazon S3.
- OpenSearch **não é obrigatório** para usar RAG.
- Lambda **não executa o modelo**, apenas orquestra a aplicação.
- EventBridge **não executa código**; ele dispara eventos.
- Bedrock continua sendo **serverless**, mesmo integrado a diversos serviços.
- SageMaker e Bedrock são serviços complementares, não concorrentes.

---

# 🔁 Resumo rápido

- Bedrock integra-se facilmente ao ecossistema AWS.
- Knowledge Bases permitem implementar RAG.
- Lambda normalmente conecta a aplicação ao Bedrock.
- S3 armazena documentos corporativos.
- OpenSearch melhora a recuperação de informações.
- IAM controla acesso.
- CloudWatch monitora.
- EventBridge automatiza fluxos.
- A arquitetura é totalmente serverless e escalável.

---

# 📌 Status de aprendizado

- [ ] Entendo a arquitetura básica do Amazon Bedrock
- [ ] Sei como funcionam as Knowledge Bases
- [ ] Entendo como o RAG utiliza documentos corporativos
- [ ] Sei quando utilizar Lambda, S3 e OpenSearch
- [ ] Conheço as principais integrações do Amazon Bedrock
- [ ] Entendo as principais considerações de segurança, desempenho e escalabilidade
