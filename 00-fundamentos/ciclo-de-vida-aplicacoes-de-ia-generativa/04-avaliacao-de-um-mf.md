# 📊 Avaliação de um Modelo de Base (FM)

<img width="911" height="105" alt="image" src="https://github.com/user-attachments/assets/4c3ba298-e130-442b-b282-0a2bf96533ed" />

Após melhorar o desempenho de um **Foundation Model (FM)**, é necessário verificar se ele realmente atende aos objetivos do negócio.

A avaliação busca responder perguntas como:

- O modelo gera respostas corretas?
- As respostas são úteis?
- O modelo é confiável?
- O desempenho atende aos requisitos da aplicação?

Uma boa avaliação combina análises humanas e métricas automatizadas.

---

# 🎯 Objetivos da Avaliação

A avaliação de um FM tem como principais objetivos:

- Verificar se o modelo atende ao caso de uso
- Medir a qualidade das respostas
- Comparar diferentes modelos
- Identificar pontos de melhoria
- Garantir que o modelo gere valor para o negócio

---

# 🛠️ Métodos de Avaliação

Existem três principais formas de avaliar um modelo de base.

## 👥 Avaliação Humana

Na avaliação humana, pessoas utilizam o modelo e analisam a qualidade das respostas produzidas.

Os avaliadores podem verificar aspectos como:

- Coerência
- Relevância
- Correção factual
- Clareza
- Qualidade geral

É considerada o **padrão-ouro (gold standard)** para avaliar modelos de IA.

### ✅ Vantagens

- Avalia aspectos subjetivos
- Detecta erros difíceis de medir automaticamente
- Aproxima-se da experiência real do usuário

### ❌ Desvantagens

- Alto custo
- Processo demorado
- Difícil de escalar

---

## 📚 Conjuntos de Dados de Referência (Benchmarks)

Os **benchmarks** são conjuntos de dados preparados especificamente para comparar modelos de IA.

Todos os modelos são avaliados utilizando exatamente os mesmos testes.

Isso permite comparar o desempenho entre diferentes modelos.

---

## Principais benchmarks

### 📖 GLUE

**General Language Understanding Evaluation**

Conjunto de tarefas para avaliar compreensão da linguagem natural.

Avalia, por exemplo:

- Classificação de texto
- Inferência textual
- Resposta a perguntas

---

### 🚀 SuperGLUE

Versão mais difícil do GLUE.

Foi criada porque muitos modelos passaram a obter resultados muito altos no GLUE.

Possui tarefas mais complexas de compreensão da linguagem.

---

### ❓ SQuAD

**Stanford Question Answering Dataset**

Benchmark utilizado para avaliar sistemas de perguntas e respostas.

O modelo deve localizar corretamente a resposta dentro de um texto.

---

### 🌍 WMT

**Workshop on Machine Translation**

Conjunto de tarefas voltado para tradução automática entre idiomas.

Muito utilizado para comparar modelos tradutores.

---

## ✅ Vantagens

- Avaliação padronizada
- Fácil comparação entre modelos
- Permite acompanhar evolução dos modelos

### ❌ Limitações

- Pode não representar situações reais
- Não mede completamente a experiência do usuário

---

## 🤖 Métricas Automatizadas

As métricas automatizadas permitem avaliar rapidamente o desempenho de um modelo.

São muito utilizadas durante o desenvolvimento para testar novas versões do modelo.

Embora sejam rápidas, normalmente não conseguem capturar toda a qualidade percebida por humanos.

---

## Principais métricas

### 📉 Perplexidade

Mede o quão bem o modelo consegue prever o próximo token.

Quanto **menor** a perplexidade:

- melhor o modelo;
- maior sua capacidade preditiva.

---

### 🌍 BLEU

**Bilingual Evaluation Understudy**

Muito utilizada para tradução automática.

Compara o texto gerado com traduções consideradas corretas.

Leva em consideração:

- Precisão
- Brevidade

Quanto maior a pontuação BLEU, mais semelhante a tradução está da referência.

---

### 🎯 F1 Score

Muito utilizada em tarefas de:

- Classificação
- Reconhecimento de entidades

Combina:

- Precisão (Precision)
- Revocação (Recall)

É especialmente útil quando existe desbalanceamento entre classes.

---

# 📈 Métricas Importantes para IA Generativa

Além das métricas anteriores, existem métricas específicas para avaliar modelos generativos.

---

## 📝 ROUGE

**Recall-Oriented Understudy for Gisting Evaluation**

Muito utilizada para:

- Resumo automático
- Tradução

Compara o texto gerado com um ou mais textos de referência.

Seu foco principal é medir quanto conteúdo relevante foi recuperado.

---

## 🌍 BLEU

Também pode ser utilizada para IA generativa.

Seu foco está na similaridade entre o texto gerado e o texto esperado.

É especialmente popular em tradução automática.

---

## 🧠 BERTScore

Utiliza embeddings produzidos por modelos BERT para comparar o significado dos textos.

Diferentemente do BLEU, não compara apenas palavras iguais.

Avalia a **semelhança semântica** entre os textos.

Isso o torna mais próximo da forma como humanos avaliam qualidade textual.

---

# ⚠️ Limitações das Métricas

Embora sejam úteis, métricas automáticas possuem limitações.

Elas podem indicar que duas respostas são diferentes mesmo quando possuem o mesmo significado.

Da mesma forma, podem considerar duas respostas semelhantes mesmo quando uma delas não atende completamente ao usuário.

Por isso, recomenda-se combinar:

- Avaliação humana
- Benchmarks
- Métricas automatizadas

---

## 🔁 Comparações importantes

---

### Avaliação Humana vs Métricas Automatizadas

| Avaliação Humana | Métricas Automatizadas |
|------------------|------------------------|
| Mais precisa | Mais rápida |
| Alto custo | Baixo custo |
| Difícil escalar | Fácil escalar |
| Avalia qualidade percebida | Avalia indicadores objetivos |

---

### Benchmarks vs Avaliação Humana

| Benchmarks | Avaliação Humana |
|------------|------------------|
| Padronizados | Subjetiva |
| Comparação entre modelos | Avaliação da experiência real |
| Fácil reprodução | Mais cara |
| Boa para pesquisa | Melhor para validar aplicações reais |

---

### ROUGE vs BLEU vs BERTScore

| ROUGE | BLEU | BERTScore |
|--------|------|-----------|
| Foca em recall | Foca em precisão | Foca em significado |
| Muito usado em resumo | Muito usado em tradução | Usa embeddings do BERT |
| Compara texto com referência | Compara similaridade textual | Compara similaridade semântica |

---

## 🧠 Conceitos importantes para prova

- Avaliação humana é considerada o **padrão-ouro**.
- Benchmarks permitem comparar modelos de forma padronizada.
- GLUE e SuperGLUE avaliam compreensão de linguagem natural.
- SQuAD avalia sistemas de perguntas e respostas.
- WMT é utilizado para tradução automática.
- Perplexidade mede a capacidade de prever o próximo token.
- ROUGE é muito utilizado para resumo automático.
- BLEU é amplamente utilizado em tradução automática.
- BERTScore mede similaridade semântica utilizando embeddings do BERT.
- A melhor prática é combinar avaliação humana e métricas automatizadas.

---

## ⚠️ Pegadinhas comuns

- Avaliação humana é a mais confiável, mas não é a mais rápida.
- BLEU não mede significado; mede similaridade entre textos.
- ROUGE é mais utilizado para resumos do que para tradução.
- BERTScore utiliza embeddings, não apenas comparação de palavras.
- Benchmarks não substituem testes em cenários reais.
- Uma métrica alta não garante que o usuário ficará satisfeito com a resposta.

---

## 🔁 Resumo rápido

- Modelos de base precisam ser avaliados antes da implantação.
- Existem três abordagens principais: avaliação humana, benchmarks e métricas automatizadas.
- Benchmarks como GLUE, SuperGLUE, SQuAD e WMT permitem comparar modelos.
- Métricas como Perplexidade, ROUGE, BLEU e BERTScore medem diferentes aspectos da qualidade.
- A combinação de avaliação humana e métricas automáticas fornece a análise mais completa.

---

## 📌 Status de aprendizado

- [ ] Entendo o objetivo da avaliação de um FM
- [ ] Sei diferenciar avaliação humana, benchmarks e métricas automatizadas
- [ ] Sei para que servem GLUE, SuperGLUE, SQuAD e WMT
- [ ] Entendo o que mede a Perplexidade
- [ ] Sei a diferença entre ROUGE, BLEU e BERTScore
- [ ] Entendo por que a avaliação humana continua sendo o padrão-ouro
