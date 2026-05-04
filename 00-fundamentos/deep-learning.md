# 🧠 Fundamentos de Deep Learning

## 📌 O que é

Deep Learning é um subcampo de Machine Learning que utiliza **redes neurais artificiais com múltiplas camadas (deep neural networks)** para aprender padrões complexos em grandes volumes de dados.

📌 É especialmente eficaz para **dados não estruturados** como imagens, áudio e texto.

---

## 🎯 Quando usar

- Quando há **grandes volumes de dados**
- Quando o problema envolve:
  - Imagens (visão computacional)
  - Texto (NLP)
  - Áudio (fala)
- Quando modelos tradicionais de ML não performam bem
- Quando há disponibilidade de **alto poder computacional (GPU/TPU)**

---

## ⚙️ Como funciona

Deep Learning utiliza redes neurais compostas por camadas:

1. Camada de entrada (input)
2. Camadas ocultas (hidden layers)
3. Camada de saída (output)

Cada camada:
- Recebe dados
- Aplica transformações matemáticas
- Passa o resultado para a próxima camada

📌 Quanto mais camadas → maior capacidade de aprender padrões complexos

---

## 🧠 Conceitos importantes

### 🧬 Redes neurais artificiais (Neural Networks)

- Inspiradas no cérebro humano
- Compostas por neurônios artificiais
- Cada neurônio:
  - Recebe entradas
  - Aplica um peso
  - Gera uma saída

---

### 🔢 Camadas (Layers)

- Input layer → recebe os dados
- Hidden layers → processam informações
- Output layer → gera resultado final

📌 Deep Learning = muitas camadas ocultas

---

### ⚖️ Pesos (Weights) e Bias

- Pesos → importância de cada entrada
- Bias → ajuste fino do modelo

📌 Treinamento = ajustar pesos e bias

---

### 🔄 Função de ativação

- Define se um neurônio "ativa" ou não
- Introduz não linearidade
- Ex:
  - ReLU
  - Sigmoid
  - Tanh

---

### 📉 Função de perda (Loss Function)

- Mede o erro do modelo
- Objetivo: minimizar o erro
- Ex:
  - Erro quadrático
  - Entropia cruzada

---

### 🔁 Backpropagation

- Algoritmo que ajusta os pesos
- Baseado no erro calculado
- Fluxo:
  1. Modelo faz previsão  
  2. Calcula erro  
  3. Ajusta pesos para reduzir erro  

---

### ⚡ Treinamento com GPU/TPU

- Deep Learning exige alto poder computacional
- GPUs/TPUs aceleram:
  - Treinamento
  - Processamento paralelo

---

### 🧩 Tipos de redes neurais

#### CNN (Convolutional Neural Network)
- Ideal para imagens
- Detecta padrões visuais

---

#### RNN (Recurrent Neural Network)
- Ideal para dados sequenciais
- Ex:
  - Texto
  - Séries temporais

---

#### Transformers
- Base dos LLMs modernos
- Excelente para NLP
- Usado em:
  - Chatbots
  - Tradução
  - Geração de texto

---

## 💰 Modelo de cobrança (conceitual)

Na AWS:

- Treinamento:
  - Muito caro (uso intensivo de GPU/TPU)
- Inferência:
  - Custo contínuo
  - Pode ser otimizado

📌 Deep Learning costuma ser mais caro que ML tradicional

---

## 🔒 Segurança (conceitual)

- Pode amplificar:
  - Bias (viés)
  - Problemas de dados
- Riscos:
  - Overfitting em dados sensíveis
  - Uso indevido de dados

---

## 🔁 Comparações importantes

---

### Machine Learning vs Deep Learning

| Machine Learning | Deep Learning |
|----------------|--------------|
| Menos dados | Precisa de muitos dados |
| Menos poder computacional | Alto poder computacional |
| Feature engineering manual | Aprende features automaticamente |
| Mais interpretável | Menos interpretável |

---

### Redes neurais vs algoritmos tradicionais

| Redes neurais | Algoritmos tradicionais |
|--------------|------------------------|
| Alta complexidade | Mais simples |
| Melhor para dados não estruturados | Melhor para dados estruturados |
| Menos interpretável | Mais interpretável |

---

## 🧠 Conceitos importantes para prova

- Deep Learning = **rede neural com múltiplas camadas**
- Funciona melhor com:
  - Muitos dados
  - Alto poder computacional
- Aprende **features automaticamente**
- Base dos:
  - LLMs
  - Generative AI
- Transformers são arquitetura moderna dominante

---

## ⚠️ Pegadinhas comuns

- Deep Learning ≠ sempre melhor (depende do problema)
- Precisa de muitos dados (poucos dados → ruim)
- Mais complexo ≠ mais eficiente
- Não é facilmente interpretável
- Alto custo computacional

---

## 🔁 Resumo rápido

- Deep Learning é um tipo de ML baseado em redes neurais profundas
- Ideal para dados não estruturados
- Aprende automaticamente padrões complexos
- Usa GPUs/TPUs para treinar
- Base da Generative AI e LLMs

---

## 📌 Status de aprendizado

- [ ] Entendo o que é Deep Learning
- [ ] Sei como redes neurais funcionam
- [ ] Entendo o papel de camadas, pesos e ativação
- [ ] Sei a diferença entre ML e Deep Learning
- [ ] Entendo quando usar Deep Learning
