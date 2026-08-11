# 🧩 Prompt Engineering

## 📌 O que é

Prompt Engineering é a prática de criar instruções (**prompts**) de forma estratégica para obter respostas mais úteis, precisas e relevantes de um modelo de IA Generativa.

Em muitos casos, **a qualidade da resposta depende diretamente da qualidade do prompt**.

📌 Um mesmo modelo pode produzir respostas completamente diferentes dependendo de como a solicitação é escrita.

---

## 🎯 Por que é importante?

Um bom prompt permite que o modelo:

- Entenda corretamente a tarefa
- Gere respostas mais precisas
- Produza saídas no formato desejado
- Reduza ambiguidades
- Diminua a necessidade de retrabalho

Na prática, muitas vezes melhorar o prompt é mais simples e barato do que realizar Fine-tuning.

---

# ⚙️ Como funciona

Em alto nível, o processo é:

```text
Prompt
    ↓
Modelo interpreta a solicitação
    ↓
Aplica o conhecimento aprendido
    ↓
Gera novos tokens
    ↓
Resposta
```

Quanto mais contexto e instruções relevantes forem fornecidos, maior tende a ser a qualidade da resposta.

---

# 🧱 Estrutura de um bom prompt

Um prompt costuma ser composto por quatro elementos principais.

---

## 📋 Instrução (Instruction)

Define claramente o que o modelo deve fazer.

Exemplos:

- Resuma o texto.
- Traduza para inglês.
- Explique este conceito.
- Gere um e-mail profissional.

📌 A instrução é a parte mais importante do prompt.

---

## 📚 Contexto (Context)

Fornece informações adicionais para orientar o modelo.

Exemplos:

- Público-alvo
- Área de atuação
- Objetivo
- Restrições
- Cenário

Quanto melhor o contexto, mais personalizada tende a ser a resposta.

---

## 📝 Dados de entrada (Input Data)

São as informações que o modelo utilizará para executar a tarefa.

Exemplos:

- Documento
- Texto
- Código
- Imagem
- Tabela
- Pergunta

---

## 📤 Formato da saída (Output Indicator)

Especifica como a resposta deve ser apresentada.

Exemplos:

- Lista
- Tabela
- JSON
- Markdown
- Texto resumido
- Passo a passo

Definir o formato evita respostas inesperadas.

---

# ✨ Exemplo

## Prompt simples

> Explique computação em nuvem.

Resposta:

- Pode variar bastante.

---

## Prompt melhorado

> Explique computação em nuvem para um estudante iniciante em até cinco tópicos utilizando linguagem simples.

Resultado esperado:

- Resposta mais objetiva
- Linguagem adequada
- Estrutura organizada

📌 Pequenas mudanças no prompt podem produzir grandes diferenças na qualidade da resposta.

---

# 🌡️ Parâmetros de inferência

Além do prompt, alguns parâmetros influenciam o comportamento do modelo.

---

## 🎯 Temperatura (Temperature)

Controla o grau de aleatoriedade da resposta.

### Temperatura baixa

Características:

- Mais previsível
- Mais consistente
- Mais determinística
- Menos criativa

Indicada para:

- Resumos
- Documentação
- Código
- Respostas técnicas

---

### Temperatura alta

Características:

- Mais criativa
- Maior variedade
- Respostas menos previsíveis

Indicada para:

- Brainstorming
- Histórias
- Marketing
- Conteúdo criativo

---

## 🔢 Top-k

O modelo olha para todas as palavras possíveis e seleciona apenas as K palavras mais prováveis.

Na prática:

- Valores menores evitam palavras sem sentido, mas deixam o texto repetitivo.
- Valores maiores permitem maior variedade de vocabulário.

**Exemplo (Top-k = 40)**: O modelo escolhe a próxima palavra apenas entre as 40 opções mais cotadas.

📌 Para a AI Practitioner, basta conhecer o conceito geral. Não é necessário decorar valores.

---

## 🔢 Top-p

O modelo junta as palavras mais prováveis até que a soma das chances delas atinja o valor de P.

Na prática:

- Valores menores tornam a resposta mais conservadora.
- Valores maiores permitem maior diversidade.

**Exemplo (Top-p = 0.9):** O modelo considera apenas o grupo de palavras cujas chances somadas chegam a 90% do total.

📌 Para a AI Practitioner, basta conhecer o conceito geral. Não é necessário decorar valores.

---

## 📏 Máximo de tokens (Max Tokens)

Define o tamanho máximo da resposta gerada.

Impacta:

- Comprimento da resposta
- Tempo de processamento
- Custo

---

# 🎯 Boas práticas

Ao criar prompts:

- Seja claro.
- Seja específico.
- Forneça contexto.
- Defina o formato esperado.
- Divida tarefas complexas em etapas menores quando necessário.

Quanto mais objetiva for a solicitação, melhor tende a ser o resultado.

---

# 🚫 Más práticas

Evite prompts:

- Muito vagos
- Ambíguos
- Sem contexto
- Com várias tarefas misturadas
- Sem especificar o resultado esperado

Exemplo ruim:

> Fale sobre tecnologia.

Exemplo melhor:

> Explique computação em nuvem para um estudante iniciante utilizando exemplos simples e uma tabela comparando nuvem pública, privada e híbrida.

---

# ☁️ Prompt Engineering no Amazon Bedrock

O Amazon Bedrock permite utilizar Prompt Engineering com qualquer Foundation Model disponível.

Além dos prompts simples, é possível combinar técnicas como:

- Bases de Conhecimento (Knowledge Bases)
- RAG (Retrieval-Augmented Generation)
- Agentes
- Fluxos (Flows)
- Guardrails

Isso permite criar aplicações muito mais robustas sem modificar o modelo.

---

# 🔁 Comparações importantes

## Prompt simples vs Prompt detalhado

| Prompt simples | Prompt detalhado |
|----------------|------------------|
| Pouco contexto | Muito contexto |
| Respostas mais genéricas | Respostas mais precisas |
| Maior ambiguidade | Menor ambiguidade |

---

## Temperatura baixa vs Alta

| Baixa temperatura | Alta temperatura |
|-------------------|------------------|
| Mais previsível | Mais criativa |
| Mais consistente | Mais variada |
| Melhor para tarefas técnicas | Melhor para tarefas criativas |

---

## Prompt Engineering vs Fine-tuning

| Prompt Engineering | Fine-tuning |
|--------------------|------------|
| Não altera o modelo | Altera o modelo |
| Rápido | Exige treinamento |
| Baixo custo | Maior custo |
| Fácil de testar | Mais complexo |

---

# 🧠 Conceitos importantes para prova

- Prompt é a entrada enviada ao modelo.
- A qualidade do prompt influencia diretamente a resposta.
- Um bom prompt normalmente contém:
  - Instrução
  - Contexto
  - Dados de entrada
  - Formato esperado da saída
- Temperatura controla criatividade.
- Max Tokens limita o tamanho da resposta.
- Prompt Engineering é uma alternativa simples e de baixo custo antes de considerar Fine-tuning.

---

# ⚠️ Pegadinhas comuns

- Um modelo melhor **não compensa** um prompt mal elaborado.
- Temperatura alta **não significa** respostas melhores.
- Prompt Engineering **não altera** os pesos do modelo.
- O mesmo prompt pode produzir respostas diferentes dependendo do modelo utilizado.
- Mais contexto costuma melhorar a resposta, mas também aumenta o consumo de tokens.

---

# 🔁 Resumo rápido

- Prompt Engineering é a criação estratégica de prompts.
- Bons prompts são claros, específicos e fornecem contexto.
- Um prompt geralmente possui:
  - Instrução
  - Contexto
  - Dados de entrada
  - Formato da saída
- Temperatura controla criatividade.
- Max Tokens limita o tamanho da resposta.
- Melhorar o prompt costuma ser mais barato do que realizar Fine-tuning.

---

# 📌 Status de aprendizado

- [ ] Entendo o que é Prompt Engineering
- [ ] Sei estruturar um bom prompt
- [ ] Entendo o papel da temperatura
- [ ] Sei o que é Max Tokens
- [ ] Conheço as principais boas práticas
- [ ] Sei a diferença entre Prompt Engineering e Fine-tuning
