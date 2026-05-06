# 💰 Considerações de custos em IA na AWS (Cost Considerations)

## 📌 O que é

Custos em IA/ML na AWS envolvem diversos fatores que impactam diretamente o preço final de uma solução, como:

- Tipo de serviço utilizado
- Volume de dados processados
- Nível de desempenho e disponibilidade
- Uso de modelos generativos

📌 Em IA, custo ≠ apenas infraestrutura → envolve também **uso do modelo**

---

## 🎯 Quando se preocupar com custos

- Sempre que estiver projetando soluções de IA/ML
- Ao escolher entre:
  - Serviços prontos vs customizados
  - Batch vs tempo real
  - Modelos simples vs complexos

- Ex:
  - Escolher entre Bedrock vs SageMaker
  - Decidir entre GPU vs CPU
  - Usar RAG vs Fine-tuning

---

## ⚙️ Como funciona

O custo em IA na AWS geralmente é baseado em:

1. Uso de computação (CPU, GPU)
2. Volume de dados processados
3. Número de requisições
4. Tokens (em Generative AI)
5. Tempo de execução

📌 Cada serviço pode ter um modelo diferente

---

## 🧠 Conceitos importantes

### ⚡ Capacidade de resposta e disponibilidade (Responsiveness & Availability)

- Serviços com:
  - Baixa latência
  - Alta disponibilidade
- Tendem a custar mais

📌 Ex:
  - Inferência em tempo real → mais caro
  - Batch → mais barato

---

### 🌍 Redundância e cobertura regional (Redundancy & Regional Coverage)

- Uso de:
  - Múltiplas AZs
  - Múltiplas Regiões

- Gera:
  - Alta disponibilidade
  - Maior custo

📌 Ex:
  - Replicação de dados
  - Deploy multi-região

---

### 🚀 Desempenho (Performance)

- Tipos de computação:
  - CPU
  - GPU
  - Aceleradores (ex: Inferentia)

- GPU:
  - Mais caro
  - Melhor para ML e Deep Learning

📌 Trade-off:
- Mais performance → mais custo

---

### 🔤 Preços baseados em tokens (Token-based Pricing)

- Usado em Generative AI (ex: Bedrock, Amazon Q)
- Você paga por:
  - Tokens de entrada (input)
  - Tokens de saída (output)

📌 Quanto mais texto gerar/processar → maior custo

---

### ⚙️ Throughput provisionado (Provisioned Throughput)

- Capacidade reservada antecipadamente
- Garante:
  - Performance previsível
  - Baixa latência

📌 Trade-off:
- Mais throughput → mais custo

- Ex:
  - Processamento de áudio contínuo
  - Aplicações críticas

---

### 🧠 Modelos personalizados (Custom Models / Fine-tuning)

- Criar ou ajustar modelos próprios gera custo adicional

- Envolve:
  - Treinamento
  - Armazenamento
  - Inferência

📌 Alternativa mais barata:
- Usar modelos pré-treinados ou RAG

---

### 📊 Volume de dados

- Mais dados → mais custo

- Impacta:
  - Treinamento
  - Inferência
  - Armazenamento

---

## 💰 Fatores que mais impactam custo

- Uso de GPU
- Tokens (Generative AI)
- Tempo de execução
- Throughput provisionado
- Deploy em múltiplas regiões
- Modelos customizados

---

## 🔁 Comparações importantes

---

### Batch vs Tempo real

| Batch | Tempo real |
|------|-----------|
| Mais barato | Mais caro |
| Alta latência | Baixa latência |
| Processamento em massa | Resposta imediata |

---

### CPU vs GPU

| CPU | GPU |
|-----|-----|
| Mais barato | Mais caro |
| Menos performance | Alta performance |
| Uso geral | ML / Deep Learning |

---

### Modelos pré-treinados vs customizados

| Pré-treinado | Customizado |
|-------------|------------|
| Mais barato | Mais caro |
| Rápido | Demorado |
| Menos flexível | Mais flexível |

---

## 🧠 Conceitos importantes para prova

- Generative AI usa **tokens como unidade de custo**
- Inferência em tempo real custa mais que batch
- GPU custa mais que CPU
- Alta disponibilidade → maior custo
- Fine-tuning é mais caro que usar modelos prontos
- Throughput provisionado aumenta custo

---

## ⚠️ Pegadinhas comuns

- Mais performance ≠ sempre melhor escolha
- Baixa latência tem custo alto
- Tokens podem crescer rapidamente
- Multi-região aumenta custo significativamente
- Customização nem sempre compensa

---

## 🔁 Resumo rápido

- Custos em IA dependem de múltiplos fatores
- Principais drivers:
  - Tokens
  - Computação (CPU/GPU)
  - Tempo de uso
- Trade-offs:
  - Performance vs custo
  - Latência vs custo
- Sempre avaliar o caso de uso

---

## 📌 Status de aprendizado

- [ ] Entendo como IA é cobrada na AWS
- [ ] Sei o impacto de tokens no custo
- [ ] Entendo CPU vs GPU
- [ ] Sei quando usar batch vs tempo real
- [ ] Entendo custos de modelos customizados
