# 📚 Geração Aumentada de Recuperação (RAG)

A **Retrieval-Augmented Generation (RAG)** é uma técnica utilizada para melhorar a qualidade das respostas geradas por um **Large Language Model (LLM)**.

Em vez de depender apenas do conhecimento adquirido durante o treinamento, o modelo consulta uma **base de conhecimento externa** para obter informações relevantes antes de gerar sua resposta.

Isso permite produzir respostas:

- Mais precisas
- Mais atualizadas
- Mais contextualizadas
- Baseadas em informações da própria empresa

---

# 🎯 Por que usar RAG?

Os LLMs são treinados utilizando enormes volumes de dados públicos.

Apesar desse conhecimento geral, eles normalmente **não possuem acesso às informações internas de uma empresa**, como:

- Documentações
- Manuais
- Procedimentos internos
- Histórico de suporte
- Políticas corporativas
- Dados específicos do negócio

Sem acesso a essas informações, o modelo pode responder de forma incorreta ou incompleta.

A RAG resolve esse problema adicionando conhecimento externo no momento da geração da resposta.

---

# 🏢 Dados empresariais

As empresas armazenam uma enorme quantidade de informações úteis.

Exemplos:

- 📄 Documentos
- 📊 Apresentações
- 📘 Manuais
- 📚 Bases de conhecimento
- 🎫 Tickets de suporte
- 💬 Conversas de chat
- 📞 Transcrições de chamadas
- 📈 Relatórios

Esses dados normalmente não fizeram parte do treinamento original do modelo.

Por isso, precisam ser disponibilizados durante a inferência por meio da RAG.

---

# ⚙️ Como a RAG funciona

O fluxo simplificado é o seguinte:

1. O usuário envia um prompt.
2. O sistema transforma o prompt em uma representação vetorial.
3. É realizada uma busca por conteúdos semelhantes na base de conhecimento.
4. Os documentos mais relevantes são recuperados.
5. Esses documentos são enviados juntamente com o prompt ao LLM.
6. O modelo gera uma resposta utilizando esse contexto adicional.

Assim, o modelo responde utilizando tanto seu conhecimento geral quanto as informações específicas recuperadas.

---

# 🧠 Incorporações vetoriais (Embeddings)

Para que seja possível localizar informações relevantes rapidamente, os textos precisam ser transformados em números.

Esse processo é chamado de **incorporação vetorial (Embedding)**.

Um modelo de Machine Learning converte textos, imagens ou áudios em vetores numéricos posicionados em um espaço multidimensional.

Esses vetores representam o significado semântico dos dados.

<img width="926" height="576" alt="image" src="https://github.com/user-attachments/assets/4495063f-20ab-45b9-ad5e-1bc965429f6f" />

---

## 🎯 Objetivo dos embeddings

O objetivo é fazer com que conteúdos semanticamente semelhantes fiquem próximos no espaço vetorial.

Por exemplo:

| Palavra | Relação semântica |
|----------|-------------------|
| Mar | Próxima de Oceano |
| Oceano | Próxima de Mar |
| Grampeador | Distante das anteriores |

Mesmo que as palavras sejam diferentes, seus vetores ficam próximos quando possuem significados semelhantes.

<img width="941" height="526" alt="image" src="https://github.com/user-attachments/assets/60a08b87-07b4-438b-8919-69bc5f686c36" />

Isso permite realizar buscas por significado, e não apenas por palavras idênticas.

---

# 🗄️ Bancos de dados vetoriais

Após gerar os embeddings, os vetores são armazenados em bancos de dados especializados chamados **Vector Databases**.

Sua principal função é:

- Armazenar bilhões de vetores
- Indexar esses vetores
- Permitir buscas extremamente rápidas por similaridade

Ao receber uma consulta, o banco encontra os vetores mais próximos do vetor da pergunta.

Esses documentos são enviados ao LLM como contexto.

---

## 🔍 Algoritmos de busca

Os algoritmos mais utilizados para encontrar vetores semelhantes são:

- k-Nearest Neighbors (k-NN)
- Similaridade de Cosseno (Cosine Similarity)

Ambos buscam identificar quais vetores possuem maior proximidade semântica com a consulta realizada.

---

# ☁️ Opções de bancos vetoriais na AWS

A AWS oferece diversas opções para armazenamento vetorial, incluindo:

- Amazon OpenSearch Service
- Amazon OpenSearch Serverless
- pgvector no Amazon RDS para PostgreSQL
- pgvector no Amazon Aurora PostgreSQL
- Amazon Kendra

Cada solução possui características próprias relacionadas a custo, escalabilidade e integração.

---

# 🏢 RAG no caso da AnyCompany

No chatbot da AnyCompany, o fluxo passa a funcionar da seguinte maneira:

<img width="959" height="615" alt="image" src="https://github.com/user-attachments/assets/155deed6-01cc-4c55-b6d0-f8f2493c7f55" />

1. O cliente faz uma pergunta.
2. A pergunta é convertida em embedding.
3. O sistema consulta a base de conhecimento da empresa.
4. Os documentos mais relevantes são recuperados.
5. Essas informações são enviadas ao LLM.
6. O modelo gera uma resposta baseada tanto no conhecimento geral quanto nos documentos recuperados.

Dessa forma, o chatbot consegue responder perguntas específicas sobre:

- Planos da empresa
- Procedimentos internos
- Produtos
- Histórico de suporte
- Políticas corporativas

Sem necessidade de retreinar o modelo.

---

# ✅ Benefícios da RAG

- Maior precisão nas respostas
- Informações atualizadas
- Menor ocorrência de alucinações
- Aproveitamento da documentação existente
- Não exige retreinamento do modelo
- Fácil atualização da base de conhecimento

---

## 🔁 Comparações importantes

---

### LLM tradicional vs LLM com RAG

| LLM tradicional | LLM com RAG |
|----------------|-------------|
| Usa apenas conhecimento do treinamento | Consulta uma base de conhecimento |
| Conhecimento pode estar desatualizado | Utiliza informações atualizadas |
| Não conhece dados internos | Conhece documentos da empresa |
| Maior risco de alucinações | Respostas mais fundamentadas |

---

### Banco de dados tradicional vs Banco vetorial

| Banco tradicional | Banco vetorial |
|------------------|----------------|
| Busca por valores exatos | Busca por similaridade semântica |
| Dados estruturados | Embeddings vetoriais |
| Consultas SQL | Busca por proximidade entre vetores |
| Ideal para registros | Ideal para IA generativa |

---

### Embedding vs Texto original

| Texto | Embedding |
|--------|-----------|
| Informação legível por humanos | Representação numérica |
| Não pode ser comparado matematicamente | Permite cálculo de similaridade |
| Usado pelo usuário | Usado pelos algoritmos de busca |

---

## 🧠 Conceitos importantes para prova

- RAG significa **Retrieval-Augmented Generation**.
- A RAG adiciona contexto ao LLM antes da geração da resposta.
- Embeddings são representações vetoriais de dados.
- Conteúdos semelhantes possuem embeddings próximos.
- Os embeddings são armazenados em bancos vetoriais.
- O banco realiza buscas por similaridade semântica.
- O LLM utiliza os documentos recuperados para gerar respostas mais precisas.

---

## ⚠️ Pegadinhas comuns

- RAG **não retreina** o modelo.
- Embeddings **não são** o texto original; são representações numéricas.
- Banco vetorial não substitui necessariamente um banco relacional.
- A RAG melhora o contexto da resposta, mas não altera os pesos do modelo.
- Similaridade é baseada em significado, e não apenas em palavras iguais.

---

## 🔁 Resumo rápido

- A RAG combina recuperação de informações com geração de texto.
- Documentos da empresa são transformados em embeddings.
- Os embeddings ficam armazenados em bancos vetoriais.
- Quando chega um prompt, o sistema recupera documentos semelhantes.
- O LLM recebe esses documentos como contexto e produz respostas mais precisas e atualizadas.

---

## 📌 Status de aprendizado

- [ ] Entendo o que é RAG
- [ ] Sei por que um LLM puro não é suficiente
- [ ] Entendo o conceito de embeddings
- [ ] Sei para que serve um banco de dados vetorial
- [ ] Entendo como a RAG melhora a qualidade das respostas
- [ ] Consigo explicar o fluxo completo da RAG
