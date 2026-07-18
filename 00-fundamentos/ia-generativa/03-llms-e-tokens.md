# 🧠 LLMs, Tokens e Embeddings

## 📌 O que são LLMs?

LLMs (**Large Language Models**) são Foundation Models especializados em compreender e gerar linguagem natural.

Eles são treinados em enormes volumes de texto e conseguem realizar diversas tarefas sem terem sido criados especificamente para cada uma delas.

Exemplos de tarefas:

- Responder perguntas
- Gerar textos
- Criar código
- Traduzir idiomas
- Resumir documentos
- Explicar conceitos

📌 Todo LLM é um Foundation Model, mas nem todo Foundation Model é um LLM.

---

## 🎯 Como um LLM funciona

Em alto nível, o processo é:

```text
Prompt
   ↓
Tokenização
   ↓
Processamento pelo modelo
   ↓
Geração de novos tokens
   ↓
Resposta final
```

Os modelos não processam palavras completas. Eles trabalham com **tokens**, que são transformados em representações numéricas chamadas **embeddings**.

---

# 🔤 Tokens

## 📌 O que são

Tokens são as menores unidades de informação processadas por um modelo de linguagem.

Um token pode representar:

- Uma palavra
- Parte de uma palavra
- Um caractere
- Um símbolo
- Um número
- Um sinal de pontuação

Exemplo:

A frase:

> Um cachorrinho é para o cachorro como um gatinho é para o gato.

Pode ser dividida aproximadamente em:

- "Um"
- "cachorrinho"
- "é"
- "para"
- "o"
- "cachorro"
- "como"
- "um"
- "gatinho"
- "é"
- "para"
- "o"
- "gato"

<img width="711" height="124" alt="image" src="https://github.com/user-attachments/assets/6d1602d6-cb0d-477b-86e7-b1754890ab5b" />

📌 A quantidade de tokens depende do modelo utilizado. Uma palavra pode ser dividida em vários tokens.

---

## 💰 Tokens e custo

Na maioria dos serviços de IA Generativa (como Amazon Bedrock), o custo é baseado na quantidade de tokens processados.

Normalmente são cobrados:

- Tokens de entrada (Input Tokens)
- Tokens de saída (Output Tokens)

Quanto mais tokens, maior o custo.

---

## 📏 Limite de tokens

Todo modelo possui uma quantidade máxima de tokens que consegue processar em uma única solicitação.

Esse limite considera:

- Prompt enviado
- Contexto da conversa
- Resposta gerada

📌 Ultrapassar esse limite pode fazer parte do contexto ser descartada.

---

# 🪟 Janela de contexto (Context Window)

A **Context Window** representa a quantidade máxima de tokens que um modelo consegue considerar ao gerar uma resposta.

Ela inclui, por exemplo:

- Prompt do usuário
- Histórico da conversa
- Informações recuperadas via RAG
- Resposta que será gerada

Quanto maior a janela de contexto:

- Mais informações o modelo consegue considerar
- Melhor pode ser a compreensão de documentos longos
- Maior tende a ser o custo e o tempo de processamento

---

# 🔗 Embeddings

## 📌 O que são

Embeddings são representações numéricas (vetores) que capturam o significado semântico de um conteúdo.

Em vez de trabalhar diretamente com palavras, os modelos trabalham com vetores.

<img width="433" height="376" alt="image" src="https://github.com/user-attachments/assets/9ee84a67-5284-4f14-9f45-f5b1a9ef924c" />

Cada palavra, frase ou documento é convertido em um vetor de números.

Esses vetores permitem que o modelo compreenda relações de significado.

---

## 🧠 Como funcionam

Palavras com significados semelhantes possuem vetores próximos.

Exemplo:

```
gato
felino
gatinho
```

Ficam próximos no espaço vetorial.

Já palavras sem relação ficam distantes.

Exemplo:

```
gato

avião
```

📌 O modelo aprende essas relações durante o treinamento.

---

## 🎯 Para que servem

Embeddings são amplamente utilizados em:

- Busca semântica
- Sistemas de recomendação
- RAG (Retrieval-Augmented Generation)
- Bases de conhecimento
- Agrupamento de documentos

Eles permitem encontrar conteúdos semelhantes mesmo quando utilizam palavras diferentes.

---

# 📝 Modalidades dos Foundation Models

Os Foundation Models podem trabalhar com diferentes tipos de dados (modalidades).

As modalidades mais comuns são:

---

## 📝 Texto

Especializados em:

- Geração de texto
- Tradução
- Resumos
- Perguntas e respostas

Exemplos:

- Amazon Nova Micro
- Claude
- Llama

---

## 🖼️ Imagem

Especializados em:

- Geração de imagens
- Edição
- Análise de imagens

Exemplos:

- Amazon Nova Canvas
- Stability AI

---

## 🔗 Embeddings

Geram representações vetoriais utilizadas em:

- Busca semântica
- Sistemas RAG
- Recuperação de documentos

📌 Eles normalmente **não geram texto**, mas produzem vetores.

---

# ☁️ LLMs no Amazon Bedrock

O Amazon Bedrock fornece acesso a diversos LLMs por meio de uma API unificada.

Alguns exemplos:

- Amazon Nova
- Amazon Titan
- Anthropic Claude
- Meta Llama
- Cohere
- AI21 Labs

Cada modelo possui características próprias, como:

- Custo
- Velocidade
- Qualidade das respostas
- Modalidades suportadas
- Janela de contexto

---

# 🔁 Comparações importantes

## Token vs Palavra

| Token | Palavra |
|--------|----------|
| Unidade processada pelo modelo | Unidade da linguagem humana |
| Pode representar parte de uma palavra | Sempre representa uma palavra completa |
| Usado para processamento e cobrança | Usado apenas para leitura humana |

---

## Foundation Model vs LLM

| Foundation Model | LLM |
|------------------|-----|
| Modelo de propósito geral | Especializado em linguagem natural |
| Pode trabalhar com texto, imagem, áudio e vídeo | Trabalha principalmente com texto |
| Base da IA Generativa | Tipo específico de Foundation Model |

---

## Token vs Embedding

| Token | Embedding |
|--------|-----------|
| Unidade de texto | Representação numérica do significado |
| É a entrada do modelo | É como o modelo representa essa entrada internamente |

---

# 🧠 Conceitos importantes para prova

- LLM significa **Large Language Model**.
- Todo LLM é um Foundation Model.
- Os modelos processam **tokens**, não palavras.
- Embeddings representam o significado dos dados em forma de vetores.
- Tokens influenciam:
  - Custo
  - Tempo de processamento
  - Limite de contexto
- Embeddings são fundamentais para busca semântica e RAG.

---

# ⚠️ Pegadinhas comuns

- Tokens **não** são palavras.
- Embeddings **não** armazenam texto, mas representações numéricas.
- Um Foundation Model pode trabalhar com modalidades além de texto.
- Uma janela de contexto maior **não significa** necessariamente respostas melhores; ela apenas permite considerar mais informações.
- Mais tokens também significam maior custo.

---

# 🔁 Resumo rápido

- LLMs são Foundation Models especializados em linguagem natural.
- Modelos processam tokens.
- Tokens são convertidos em embeddings.
- Embeddings representam significado semântico.
- A janela de contexto limita quantos tokens o modelo consegue considerar.
- Tokens influenciam custo, desempenho e capacidade do modelo.

---

# 📌 Status de aprendizado

- [ ] Entendo o que é um LLM
- [ ] Sei a diferença entre LLM e Foundation Model
- [ ] Entendo o conceito de tokens
- [ ] Sei como tokens influenciam custo e contexto
- [ ] Entendo o que são embeddings
- [ ] Sei para que embeddings são utilizados
