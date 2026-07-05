# 📊 Avaliação dos Resultados (RAG)

Avaliar o desempenho de uma aplicação baseada em **RAG (Retrieval-Augmented Generation)** é uma etapa essencial para garantir que o modelo produza respostas **precisas, relevantes e úteis** para os usuários.

Como aplicações RAG combinam um **LLM** com uma **base de conhecimento**, a avaliação deve considerar tanto a qualidade da geração quanto a eficiência da recuperação das informações.

Os dois métodos de avaliação mais utilizados são:

- 👤 Avaliação humana
- 📚 Conjuntos de dados de referência (Benchmarks)

Na prática, ambos são utilizados de forma complementar.

---

# 👤 Avaliação humana

A avaliação humana consiste em permitir que pessoas reais interajam com o sistema e forneçam feedback sobre sua qualidade.

Esse método é importante porque existem características que apenas um usuário consegue avaliar adequadamente.

## 🎯 O que é avaliado

### 😊 Experiência do usuário

Avalia se a interação é agradável, intuitiva e útil.

Exemplos:

- Facilidade de uso
- Clareza das respostas
- Naturalidade da conversa
- Satisfação do usuário

---

### 💬 Adequação contextual

Verifica se o modelo compreendeu corretamente o contexto da conversa.

Avalia se as respostas são:

- Relevantes
- Coerentes
- Consistentes com a pergunta
- Adequadas ao cenário apresentado

---

### 🎨 Criatividade e flexibilidade

Avalia como o modelo responde a situações não previstas durante o treinamento.

Exemplos:

- Perguntas incomuns
- Problemas complexos
- Situações ambíguas
- Consultas com múltiplas interpretações

---

## ✅ Vantagens

- Avalia aspectos subjetivos
- Mede a experiência real dos usuários
- Ajuda no refinamento contínuo da aplicação

## ⚠️ Desvantagens

- Processo lento
- Alto custo
- Difícil de escalar
- Pode sofrer influência da opinião do avaliador

---

# 📚 Conjuntos de dados de referência (Benchmarks)

Os conjuntos de dados de referência permitem realizar uma avaliação **objetiva e padronizada** do modelo.

Eles consistem em perguntas e respostas previamente definidas, utilizadas para verificar se o modelo produz os resultados esperados.

Esse tipo de avaliação é muito utilizado antes da implantação da aplicação em produção.

---

## 📏 Principais métricas

### 🎯 Precisão

Avalia se a resposta produzida está correta.

---

### ⚡ Velocidade e eficiência

Mede o tempo necessário para gerar uma resposta.

É importante principalmente em aplicações de atendimento em tempo real.

---

### 📈 Escalabilidade

Verifica se o modelo mantém um bom desempenho mesmo com:

- Grande volume de usuários
- Grande volume de consultas
- Aumento da carga de processamento

---

## ✅ Vantagens

- Avaliação objetiva
- Fácil automação
- Permite comparar diferentes modelos
- Excelente para testes contínuos

## ⚠️ Desvantagens

- Não mede qualidade da experiência do usuário
- Não avalia nuances da comunicação humana

---

# 🛠️ Como criar um conjunto de dados de referência

A criação de um benchmark normalmente é realizada por **especialistas no domínio (SMEs - Subject Matter Experts)**.

---

## 1️⃣ Criar perguntas relevantes

Os especialistas elaboram perguntas importantes relacionadas ao domínio da aplicação.

As perguntas devem ser:

- Representativas
- Relevantes
- Desafiadoras

---

## 2️⃣ Identificar o contexto

Para cada pergunta, os especialistas selecionam os documentos ou trechos que contêm a informação correta.

Esse contexto servirá como base para a resposta esperada.

---

## 3️⃣ Elaborar as respostas

Os especialistas produzem as respostas consideradas corretas.

Essas respostas tornam-se o padrão utilizado para avaliar o desempenho do sistema RAG.

---

# ⚖️ LLM como juiz (LLM as a Judge)

Após a criação do conjunto de dados de referência, a avaliação pode ser automatizada utilizando outro modelo de IA.

Essa abordagem é conhecida como **LLM como juiz**.

Nesse processo, um modelo independente compara as respostas produzidas pelo sistema avaliado com as respostas elaboradas pelos especialistas.

---

## 🔄 Funcionamento

<img width="1115" height="432" alt="image" src="https://github.com/user-attachments/assets/a03ec331-64c5-4738-b7f5-d6b333e8abfc" />

### 1️⃣ Lista de perguntas

As mesmas perguntas do benchmark são enviadas ao modelo.

---

### 2️⃣ Conjunto de dados de referência

Contém:

- Perguntas
- Contexto
- Respostas elaboradas pelos especialistas

---

### 3️⃣ Respostas geradas

O sistema RAG responde às perguntas utilizando sua base de conhecimento.

---

### 4️⃣ Modelo juiz

Um segundo LLM compara:

- Resposta esperada
- Resposta produzida

---

### 5️⃣ Pontuação de avaliação

O modelo juiz calcula uma nota considerando critérios como:

- 🎯 Precisão
- 📌 Relevância
- 📖 Abrangência

Essa avaliação automatizada facilita testes frequentes durante o desenvolvimento.

---

# 🤝 Abordagem combinada

Nenhum método de avaliação é suficiente sozinho.

Na prática, utiliza-se uma combinação de avaliações automáticas e humanas.

## Fluxo típico

1. Criar um benchmark.
2. Avaliar automaticamente utilizando métricas e LLM como juiz.
3. Implantar o sistema.
4. Coletar feedback dos usuários.
5. Melhorar continuamente o modelo.

Essa abordagem garante que o sistema seja tecnicamente eficiente e, ao mesmo tempo, ofereça uma boa experiência aos usuários.

---

# 🏢 Caso de uso: AnyCompany

<img width="956" height="521" alt="image" src="https://github.com/user-attachments/assets/8de5156f-2d72-4306-aad2-6c09fd67dfc2" />

Antes de disponibilizar o chatbot aos clientes, a **AnyCompany** realiza testes utilizando conjuntos de dados de referência.

Esses testes verificam se o chatbot responde corretamente às dúvidas mais comuns utilizando a base de conhecimento corporativa.

Após a implantação, usuários reais passam a utilizar o chatbot.

O feedback coletado durante essas interações é utilizado para:

- Melhorar a precisão das respostas
- Identificar falhas
- Aprimorar continuamente a aplicação

Dessa forma, a empresa combina avaliações automatizadas e humanas para evoluir constantemente seu sistema RAG.

---

## 🔁 Comparações importantes

---

### Avaliação humana vs Benchmark

| Avaliação humana | Benchmark |
|------------------|-----------|
| Subjetiva | Objetiva |
| Avalia experiência do usuário | Avalia desempenho técnico |
| Mais lenta | Mais rápida |
| Mais cara | Mais barata |
| Difícil de escalar | Fácil de automatizar |

---

### Benchmark tradicional vs LLM como juiz

| Benchmark tradicional | LLM como juiz |
|------------------------|---------------|
| Comparação manual | Comparação automatizada |
| Maior esforço humano | Maior escalabilidade |
| Mais lento | Mais rápido |
| Ideal para pequenas avaliações | Ideal para avaliações contínuas |

---

## 🧠 Conceitos importantes para prova

- Aplicações RAG devem ser avaliadas antes e depois da implantação.
- A avaliação humana mede aspectos qualitativos da interação.
- Benchmarks medem o desempenho técnico do sistema.
- SMEs criam perguntas, contexto e respostas de referência.
- O **LLM como juiz** automatiza a comparação entre respostas esperadas e geradas.
- A melhor estratégia combina avaliação automática com feedback humano.

---

## ⚠️ Pegadinhas comuns

- Benchmark **não substitui** avaliação humana.
- Avaliação humana **não é totalmente objetiva**.
- LLM como juiz utiliza **outro modelo** para avaliar respostas.
- Benchmarks precisam ser criados por especialistas no domínio.
- Um modelo com ótima precisão técnica pode ainda oferecer uma experiência ruim ao usuário.

---

## 🔁 Resumo rápido

- Avaliar um sistema RAG é fundamental para garantir qualidade.
- Existem dois métodos principais: avaliação humana e benchmarks.
- Benchmarks utilizam perguntas e respostas criadas por especialistas.
- O LLM como juiz automatiza a comparação entre respostas.
- A combinação de avaliações automáticas e humanas produz os melhores resultados.
- A AnyCompany utiliza benchmarks antes da produção e feedback humano após a implantação.

---

## 📌 Status de aprendizado

- [ ] Entendo por que aplicações RAG precisam ser avaliadas
- [ ] Sei diferenciar avaliação humana e benchmark
- [ ] Entendo como criar um conjunto de dados de referência
- [ ] Sei como funciona a abordagem LLM como juiz
- [ ] Entendo como a AnyCompany avalia seu chatbot
