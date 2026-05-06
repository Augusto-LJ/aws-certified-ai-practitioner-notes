# 🧩 Serviços Especializados de AI/ML (AWS Specialized AI Services)

## 📌 O que é

Serviços especializados são soluções de AI/ML da AWS voltadas para **casos de uso específicos**, geralmente mais avançados ou nichados.

📌 Diferente dos AI Services:
- Mais direcionados a problemas específicos
- Alguns exigem configuração ou entendimento maior
- Menos cobrados em prova (baixo a médio foco)

---

## 🎯 Quando usar

- Quando há necessidade de **soluções mais específicas**
- Quando os AI Services não atendem completamente
- Para acelerar desenvolvimento em cenários mais complexos

- Ex:
  - Busca inteligente em documentos
  - Recomendação personalizada
  - Experimentação com ML
  - Uso de foundation models prontos

---

## ⚙️ Como funciona

- Serviços pré-construídos para casos específicos
- Podem envolver:
  - Dados próprios
  - Configuração adicional
  - Integração com outros serviços AWS

📌 Mais flexíveis que AI Services, porém menos que SageMaker

---

## 🧠 Conceitos importantes

### 🎯 Foco em caso de uso

- Cada serviço resolve um problema bem definido
- Não são genéricos

📌 Ex:
- Busca → Kendra
- Recomendação → Personalize

---

### ⚖️ Nível intermediário de complexidade

- Mais simples que SageMaker
- Mais complexos que AI Services

---

## 📦 Serviços

---

### 🔍 Amazon Kendra

- Serviço de busca inteligente (enterprise search)
- Usa NLP para entender consultas

- Ex:
  - Busca em documentos internos
  - FAQs corporativos

📌 Vai além de busca por palavra-chave (busca semântica)

---

### 🎯 Amazon Personalize

- Sistema de recomendação personalizado

- Ex:
  - Produtos recomendados (e-commerce)
  - Conteúdo sugerido (streaming)

📌 Similar ao que Netflix/Amazon usam

---

### 🏎️ AWS DeepRacer

- Plataforma para aprender ML com carros autônomos simulados
- Usa reinforcement learning

- Ex:
  - Treinamento educacional
  - Competições

📌 Foco educacional (baixo impacto na prova)

---

### 🚀 SageMaker JumpStart

- Biblioteca de modelos e soluções prontas dentro do SageMaker
- Inclui:
  - Modelos pré-treinados
  - Foundation Models
  - Templates

- Ex:
  - Deploy rápido de modelos
  - Testar soluções sem começar do zero

📌 Acelera desenvolvimento no SageMaker

---

## 💰 Modelo de cobrança

- Baseado em uso:
  - Processamento
  - Dados
  - Recursos utilizados

📌 Pode variar bastante por serviço

---

## 🔒 Segurança

- Integração com:
  - IAM
- Dados podem ser usados para:
  - Treinamento
  - Personalização

📌 Responsabilidade sobre os dados continua sendo do usuário

---

## 🔁 Comparações importantes

---

### AI Services vs Serviços Especializados

| AI Services | Serviços Especializados |
|------------|------------------------|
| Uso geral | Casos específicos |
| Muito simples | Intermediário |
| Sem configuração | Alguma configuração |

---

### SageMaker vs Serviços Especializados

| SageMaker | Serviços Especializados |
|----------|------------------------|
| Total controle | Foco específico |
| Alta complexidade | Média complexidade |

---

## 🧠 Conceitos importantes para prova

- Serviços especializados resolvem **problemas específicos**
- Kendra → busca inteligente
- Personalize → recomendação
- JumpStart → modelos prontos no SageMaker
- DeepRacer → aprendizado de ML (educacional)

📌 Menos cobrados que:
- Bedrock
- SageMaker
- AI Services

---

## ⚠️ Pegadinhas comuns

- Kendra ≠ mecanismo de busca simples (é semântico)
- Personalize ≠ ML genérico (é recomendação)
- DeepRacer não é serviço de produção
- JumpStart não é serviço separado (faz parte do SageMaker)

---

## 🔁 Resumo rápido

- Serviços focados em casos específicos
- Nível intermediário de complexidade
- Usados para acelerar soluções prontas
- Menor prioridade na prova

---

## 📌 Status de aprendizado

- [ ] Sei o que são serviços especializados
- [ ] Sei quando usar Kendra
- [ ] Sei quando usar Personalize
- [ ] Entendo o papel do JumpStart
- [ ] Sei que DeepRacer é educacional
