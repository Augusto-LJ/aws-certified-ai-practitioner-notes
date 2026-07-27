# ⚡ Inferência (Inference)

## 📌 O que é

Inferência (Inference) é a etapa em que um modelo de Machine Learning **já treinado** é utilizado para fazer previsões ou tomar decisões com **novos dados**.

É nesse momento que o modelo passa a gerar valor para a aplicação.

📌 **Treinamento ensina o modelo; inferência utiliza o que ele aprendeu.**

---

## 🎯 Quando usar

A inferência acontece sempre que um modelo precisa realizar previsões em produção.

Exemplos:

- Classificar um e-mail como spam ou não spam
- Recomendar produtos para um cliente
- Detectar uma possível fraude em uma transação
- Prever o preço de um imóvel

---

## ⚙️ Como funciona

O processo de inferência é simples:

1. Um novo dado é enviado ao modelo
2. O modelo aplica os padrões aprendidos durante o treinamento
3. O modelo retorna uma previsão ou decisão

📌 Durante a inferência, **o modelo não aprende nem altera seus parâmetros**.

---

## 🧠 Tipos de inferência

### 📦 Inferência em lote (Batch Inference)

A inferência em lote processa **grandes volumes de dados de uma só vez**.

É indicada quando a velocidade da resposta não é tão importante quanto o processamento de muitos registros.

Características:

- Processa muitos dados simultaneamente
- Maior latência
- Geralmente possui menor custo por previsão
- Muito utilizada em processamentos periódicos

Exemplos:

- Geração de relatórios
- Análise de grandes volumes de dados
- Atualização periódica de recomendações

📌 Ideal quando a tomada de decisão imediata não é necessária.

---

### ⚡ Inferência em tempo real (Real-Time Inference)

Na inferência em tempo real, cada solicitação é processada imediatamente após ser recebida.

Características:

- Resposta imediata
- Baixa latência
- Atende uma solicitação por vez
- Indispensável para aplicações interativas

Exemplos:

- Chatbots
- Sistemas de recomendação
- Detecção de fraude
- Assistentes virtuais

📌 Ideal para aplicações em que a tomada de decisão imediata é fundamental.

---

## 📊 Batch vs Real-Time

| Inferência em lote | Inferência em tempo real |
|--------------------|--------------------------|
| Processa muitos dados de uma vez | Processa cada solicitação individualmente |
| Alta latência | Baixa latência |
| Geralmente menor custo | Geralmente maior custo |
| Processamento periódico | Resposta imediata |

---

## 💰 Modelo de cobrança (conceitual)

Na AWS, normalmente existem dois tipos de custo relacionados ao Machine Learning:

- **Treinamento:** custo elevado devido ao processamento intenso
- **Inferência:** custo contínuo conforme o modelo é utilizado em produção

📌 Em muitos cenários, o modelo é treinado poucas vezes e utilizado milhares ou milhões de vezes para inferência.

---

## 🔒 Considerações importantes

Durante a inferência:

- O modelo utiliza apenas o conhecimento adquirido no treinamento
- A qualidade das previsões depende da qualidade do treinamento
- Novos dados não alteram automaticamente o modelo

Caso o desempenho diminua ao longo do tempo, normalmente é necessário realizar um **novo treinamento (retreinamento)**.

---

## 🔁 Comparações importantes

### Treinamento vs Inferência

| Treinamento | Inferência |
|--------------|------------|
| Ensina o modelo | Utiliza o modelo treinado |
| Ajusta parâmetros internos | Não altera o modelo |
| Exige grande volume de dados | Usa novos dados para prever |
| Geralmente ocorre poucas vezes | Pode ocorrer continuamente |

---

### Batch vs Real-Time

| Batch | Real-Time |
|--------|-----------|
| Alta latência | Baixa latência |
| Processa muitos registros | Processa uma solicitação por vez |
| Mais econômico para grandes volumes | Melhor experiência para o usuário |
| Execução periódica | Execução sob demanda |

---

## 🧠 Conceitos importantes para prova

- Inferência = utilização do modelo treinado
- Durante a inferência o modelo **não aprende**
- Batch Inference processa grandes volumes de dados
- Real-Time Inference responde imediatamente
- Treinamento e inferência possuem custos diferentes
- Um modelo pode ser treinado uma única vez e realizar milhões de inferências

---

## ⚠️ Pegadinhas comuns

- Inferência **não é treinamento**
- Inferência não altera os pesos do modelo
- Tempo real **não é sempre a melhor opção**; depende do caso de uso
- Batch não significa menor qualidade, apenas maior latência
- Um modelo pode precisar ser retreinado mesmo continuando realizando inferências

---

## 🔁 Resumo rápido

- Inferência é o uso do modelo treinado para fazer previsões
- Existem dois tipos principais:
  - Batch Inference
  - Real-Time Inference
- O modelo não aprende durante a inferência
- A escolha entre batch e tempo real depende da necessidade de latência e volume de processamento

---

## 📌 Status de aprendizado

- [ ] Sei o que é inferência
- [ ] Entendo a diferença entre treinamento e inferência
- [ ] Sei diferenciar Batch Inference e Real-Time Inference
- [ ] Entendo quando utilizar cada tipo de inferência
