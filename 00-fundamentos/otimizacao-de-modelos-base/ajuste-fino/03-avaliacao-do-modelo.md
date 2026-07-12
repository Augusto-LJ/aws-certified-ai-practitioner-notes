# 📊 Avaliação do Modelo

Avaliar um modelo de linguagem é essencial para verificar se ele está produzindo respostas de qualidade e atendendo aos objetivos da aplicação.

Em tarefas de **geração de texto**, como descrições de produtos, resumos ou traduções, normalmente compara-se o texto gerado pelo modelo com um **texto de referência criado por humanos**.

As três métricas mais utilizadas para esse tipo de avaliação são:

- 📝 ROUGE
- 🌍 BLEU
- 🧠 BERTScore

Cada uma avalia aspectos diferentes da qualidade da saída.

---

# 📝 ROUGE

**ROUGE (Recall-Oriented Understudy for Gisting Evaluation)** é um conjunto de métricas utilizado principalmente para avaliar:

- Sumarização automática
- Tradução automática
- Geração de texto

Seu objetivo é medir **quanto do conteúdo da referência foi recuperado pelo modelo**, ou seja, possui foco em **recall**.

---

## 🔍 Como funciona

O ROUGE compara o texto gerado com um ou mais textos de referência escritos por humanos.

Ele mede a sobreposição de:

- Palavras
- N-gramas
- Sequências de palavras
- Fragmentos de frases

Quanto maior essa sobreposição, maior tende a ser a pontuação.

---

## 📏 Principais variantes

### 🔹 ROUGE-N

Mede a sobreposição de **N-gramas** entre os textos.

Exemplos:

- ROUGE-1 → unigramas
- ROUGE-2 → bigramas
- ROUGE-3 → trigramas

É utilizado para verificar:

- Fluência do texto
- Presença das principais informações da referência

---

### 🔹 ROUGE-L

Utiliza a **Longest Common Subsequence (LCS)**, ou seja, a maior sequência comum entre os textos.

Essa métrica avalia melhor:

- Coerência
- Ordem das informações
- Estrutura narrativa

---

## ✅ Vantagens

- Fácil de calcular
- Fácil de interpretar
- Muito utilizada em sumarização automática
- Possui boa correlação com avaliações humanas

## ⚠️ Limitações

- Baseia-se em sobreposição de palavras
- Não compreende significado semântico
- Pode penalizar paráfrases corretas

---

# 🌍 BLEU

**BLEU (Bilingual Evaluation Understudy)** é uma métrica criada para avaliar **tradução automática**, mas também pode ser utilizada em outras tarefas de geração de texto.

Seu foco é medir a **precisão** da resposta gerada.

Enquanto o ROUGE pergunta:

> "Quanto da resposta correta foi recuperado?"

O BLEU pergunta:

> "Quanto do texto gerado corresponde ao texto esperado?"

---

## 🔍 Como funciona

O BLEU compara os N-gramas do texto gerado com um ou mais textos de referência.

São analisados normalmente:

- Unigramas
- Bigramas
- Trigramas
- Quadrigramas

Além disso, aplica uma **penalidade de brevidade (Brevity Penalty)** para evitar que respostas muito curtas obtenham notas altas apenas por coincidência.

---

## ✅ Vantagens

- Muito utilizada em tradução automática
- Fácil automação
- Excelente para comparar diferentes modelos

## ⚠️ Limitações

- Não avalia significado
- Não mede criatividade
- Pode penalizar respostas corretas escritas de forma diferente

---

# 🧠 BERTScore

O **BERTScore** utiliza modelos pré-treinados, como o **BERT**, para avaliar a **similaridade semântica** entre os textos.

Diferentemente do ROUGE e do BLEU, ele **não depende apenas da correspondência exata entre palavras**.

---

## 🔍 Como funciona

O modelo transforma cada palavra em uma **embedding contextualizada**.

Em seguida, calcula a **similaridade do cosseno** entre as embeddings do texto gerado e do texto de referência.

Assim, consegue identificar quando duas respostas possuem o **mesmo significado**, mesmo utilizando palavras diferentes.

---

## ✅ Vantagens

- Avalia significado semântico
- Reconhece sinônimos
- Tolera paráfrases
- Possui maior correlação com a percepção humana

## ⚠️ Limitações

- Maior custo computacional
- Mais complexo que ROUGE e BLEU

---

# ⚖️ Comparando as métricas

| Métrica | Principal objetivo | Melhor aplicação |
|----------|--------------------|------------------|
| 📝 ROUGE | Recall (recuperação das informações) | Resumos e geração de texto |
| 🌍 BLEU | Precisão das palavras geradas | Tradução automática |
| 🧠 BERTScore | Similaridade semântica | IA generativa e recomendações |

---

# 🏢 Caso de uso: AnyCompany

A **AnyCompany**, uma varejista de moda on-line, utilizou um **LLM ajustado** para:

- Gerar descrições personalizadas de produtos
- Fazer recomendações de compra
- Melhorar a experiência dos clientes

Para verificar se o modelo realmente melhorava os resultados, diferentes métricas foram utilizadas.

<img width="1130" height="559" alt="image" src="https://github.com/user-attachments/assets/40041742-a744-471f-ab01-68088c972719" />

---

## 📝 ROUGE

O ROUGE foi utilizado para verificar se as descrições geradas continham as informações importantes presentes nas descrições de referência.

O objetivo era garantir:

- Integridade das informações
- Cobertura das características do produto
- Qualidade do conteúdo

---

## 🌍 BLEU

O BLEU foi utilizado juntamente com o ROUGE para verificar se:

- Termos importantes apareciam corretamente
- Características técnicas eram preservadas
- Frases relevantes eram mantidas

Isso ajudou a garantir descrições mais precisas e persuasivas.

---

## 🧠 BERTScore

O BERTScore foi utilizado para avaliar as recomendações de produtos.

Como ele mede a similaridade semântica, consegue verificar se os produtos recomendados realmente fazem sentido para cada cliente, mesmo quando diferentes palavras são utilizadas.

---

# 📈 Resultados obtidos

Após a implantação da solução baseada em IA generativa, a AnyCompany observou melhorias significativas nas métricas de negócio.

## 📊 Taxa de conversão

- 📈 Aumento de **15%**
- 📝 ROUGE médio de **0,85**

A alta pontuação de ROUGE indicou que as descrições continham praticamente todas as informações importantes dos produtos.

---

## 🛒 Valor médio dos pedidos

- 📈 Aumento de **20%**
- 🌍 BLEU médio de **0,78**

A precisão das descrições ajudou os clientes a tomarem decisões de compra com maior confiança.

---

## ❤️ Retenção de clientes

- 📈 Aumento de **25%**
- 🧠 BERTScore médio de **0,90**

A alta similaridade semântica mostrou que as recomendações eram altamente relevantes e personalizadas para cada cliente.

---

# 🎯 Conclusão

As três métricas contribuíram para validar diferentes aspectos do modelo:

- 📝 ROUGE confirmou que as informações importantes eram preservadas.
- 🌍 BLEU garantiu precisão na linguagem utilizada.
- 🧠 BERTScore verificou que as recomendações faziam sentido semanticamente.

Como resultado, a AnyCompany conseguiu:

- Reduzir o abandono de carrinhos
- Aumentar o valor médio das compras
- Melhorar a retenção de clientes
- Oferecer uma experiência de compra mais personalizada

---

# 🔁 Comparações importantes

### ROUGE vs BLEU

| ROUGE | BLEU |
|--------|------|
| Foco em **recall** | Foco em **precisão** |
| Mede quanto da informação foi recuperada | Mede quanto da resposta corresponde à referência |
| Muito usado em resumos | Muito usado em tradução |

---

### BLEU vs BERTScore

| BLEU | BERTScore |
|------|-----------|
| Compara palavras e N-gramas | Compara significado semântico |
| Penaliza paráfrases | Reconhece sinônimos e paráfrases |
| Mais simples | Mais sofisticado |

---

### ROUGE vs BERTScore

| ROUGE | BERTScore |
|--------|-----------|
| Avalia sobreposição lexical | Avalia similaridade semântica |
| Não entende contexto | Considera o contexto das palavras |
| Mais rápido | Mais preciso em IA generativa |

---

## 🧠 Conceitos importantes para prova

- ROUGE possui foco em **recall**.
- BLEU possui foco em **precisão**.
- BERTScore utiliza **embeddings contextualizadas** para comparar significado.
- BERTScore é menos sensível ao uso de sinônimos e paráfrases.
- As três métricas são frequentemente utilizadas em conjunto.
- Nenhuma métrica substitui completamente a avaliação humana.

---

## ⚠️ Pegadinhas comuns

- ROUGE **não mede significado**, apenas sobreposição textual.
- BLEU **não é a melhor métrica para avaliar personalização**.
- BERTScore **não depende de palavras idênticas**, mas do significado.
- Uma pontuação alta em uma métrica não garante uma boa experiência para o usuário.
- As métricas quantitativas devem ser complementadas por avaliações humanas.

---

## 🔁 Resumo rápido

- Modelos generativos são avaliados comparando suas respostas com referências humanas.
- ROUGE mede a recuperação das informações (**recall**).
- BLEU mede a precisão da resposta gerada (**precision**).
- BERTScore mede a similaridade semântica utilizando embeddings.
- A combinação das três métricas fornece uma avaliação mais completa do modelo.
- A AnyCompany utilizou essas métricas para validar melhorias nas descrições de produtos e recomendações personalizadas.

---

## 📌 Status de aprendizado

- [ ] Sei quando utilizar ROUGE
- [ ] Sei quando utilizar BLEU
- [ ] Entendo como funciona o BERTScore
- [ ] Consigo diferenciar recall, precisão e similaridade semântica
- [ ] Entendo como a AnyCompany utilizou essas métricas para avaliar seu modelo
