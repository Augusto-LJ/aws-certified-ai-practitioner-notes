# 🛠️ Ferramentas AWS para IA Responsável

## 📌 O que é

A AWS oferece diversos serviços e ferramentas para ajudar organizações a implementar práticas de **IA Responsável (Responsible AI)** durante todo o ciclo de vida dos modelos.

Essas ferramentas auxiliam em áreas como:

- Avaliação de modelos
- Proteção para IA generativa
- Detecção de viés
- Explicabilidade
- Monitoramento
- Revisão humana
- Governança
- Transparência

📌 Na certificação AI Practitioner, é importante conhecer **o propósito principal de cada serviço**, sem a necessidade de aprofundar sua implementação.

---

# 🤖 Amazon Bedrock

<img width="191" height="189" alt="image" src="https://github.com/user-attachments/assets/6d73998a-e1a6-4aea-8566-04077663c596" />

Serviço totalmente gerenciado para trabalhar com **Foundation Models (FMs)**.

Permite:

- Utilizar modelos de diversos fornecedores
- Personalizar modelos
- Criar aplicações de IA generativa
- Implementar controles de IA responsável

### Benefícios

- Sem gerenciamento de infraestrutura
- API unificada
- Segurança integrada
- Recursos de governança e proteção

📌 Principal serviço da AWS para desenvolvimento de aplicações de IA generativa.

---

# 🧠 Amazon SageMaker

<img width="189" height="190" alt="image" src="https://github.com/user-attachments/assets/aaeb1987-18f0-455d-a2aa-66409a0061fe" />

Serviço totalmente gerenciado para criação, treinamento e implantação de modelos de Machine Learning.

Permite:

- Criar modelos de ML
- Treinar modelos em escala
- Implantar modelos em produção
- Monitorar modelos
- Aplicar práticas de IA responsável

### Benefícios

- Ambiente totalmente gerenciado
- Escalabilidade automática
- Integração com ferramentas de governança
- Recursos de monitoramento e explicabilidade

📌 Enquanto o **Bedrock** é voltado para IA generativa, o **SageMaker** é a principal plataforma de Machine Learning da AWS.

---

# 🔍 Amazon SageMaker Clarify

Ferramenta voltada para avaliação de modelos e IA responsável.

Permite analisar:

- Viés (Bias)
- Explicabilidade
- Precisão
- Robustez
- Toxicidade

Também oferece suporte para:

- Avaliações automáticas
- Avaliações humanas

### Principais recursos

- Identificação de vieses nos dados e nos modelos
- Explicação das previsões
- Geração de relatórios
- Apoio à avaliação de modelos

📌 É uma das ferramentas mais importantes da AWS para IA responsável.

---

# ⚖️ SageMaker Data Wrangler

Ferramenta utilizada para preparação e tratamento de dados.

Ajuda a reduzir problemas relacionados a conjuntos de dados desbalanceados.

### Técnicas suportadas

- Subamostragem aleatória
- Sobreamostragem aleatória
- SMOTE (Synthetic Minority Oversampling Technique)

### Benefícios

- Melhor qualidade dos dados
- Melhor capacidade de generalização
- Redução de vieses causados por dados desbalanceados

---

# 🧪 SageMaker Experiments

Ferramenta utilizada para gerenciamento de experimentos de Machine Learning.

Permite:

- Comparar experimentos
- Gerenciar versões
- Registrar execuções de treinamento
- Analisar resultados

Trabalha integrada ao SageMaker Clarify.

---

# 📊 SageMaker Model Monitor

Monitora modelos já implantados em produção.

Detecta:

- Queda de desempenho
- Mudanças nos dados (Data Drift)
- Mudanças no comportamento do modelo

### Benefícios

- Monitoramento contínuo
- Alertas automáticos
- Correções preventivas

📌 Ajuda a identificar quando um modelo precisa ser reavaliado ou atualizado.

---

# 👤 Amazon A2I (Amazon Augmented AI)

Serviço utilizado para inserir revisão humana em aplicações de IA.

Permite:

- Aprovação humana
- Revisão de decisões críticas
- Fluxos **Human-in-the-Loop (HITL)**

### Casos de uso

- Aprovação de documentos
- Revisão de respostas da IA
- Validação de previsões importantes

📌 **A2I = Human Review.**

---

# 🔑 SageMaker Role Manager

Ferramenta para gerenciamento de permissões no SageMaker.

Permite:

- Gerenciar acessos
- Aplicar o princípio do menor privilégio
- Controlar permissões dos usuários

Contribui para a governança e segurança dos modelos.

---

# 📝 SageMaker Model Cards

Ferramenta para documentação dos modelos de IA.

Armazena informações como:

- Objetivo do modelo
- Casos de uso
- Dados utilizados
- Processo de treinamento
- Riscos conhecidos
- Limitações

### Benefícios

- Facilita auditorias
- Melhora a governança
- Centraliza documentação

---

# 📈 SageMaker Model Dashboard

Painel centralizado para gerenciamento dos modelos.

Permite:

- Monitorar modelos
- Visualizar métricas
- Acompanhar riscos
- Centralizar informações de governança

---

# 📚 AWS AI Service Cards

Documentação oficial dos serviços de IA da AWS.

Objetivos:

- Melhorar a transparência
- Explicar limitações
- Apresentar casos de uso
- Apoiar práticas de IA responsável

Cada AI Service Card normalmente apresenta:

- Conceitos básicos
- Casos de uso recomendados
- Limitações
- Considerações sobre IA responsável
- Boas práticas

---

## 🔁 Comparações importantes

### Amazon Bedrock vs Amazon SageMaker

| Amazon Bedrock | Amazon SageMaker |
|----------------|------------------|
| IA Generativa | Machine Learning |
| Foundation Models | Modelos personalizados |
| API unificada | Plataforma completa de ML |
| Pouca necessidade de conhecimento em ML | Mais flexível para cientistas de dados |

---

### SageMaker Clarify vs Model Monitor

| SageMaker Clarify | Model Monitor |
|-------------------|---------------|
| Avalia modelos | Monitora modelos em produção |
| Detecta viés | Detecta Data Drift |
| Explica previsões | Detecta degradação de desempenho |

---

### Model Cards vs AI Service Cards

| Model Cards | AI Service Cards |
|--------------|------------------|
| Documentam modelos criados pela organização | Documentam serviços de IA da AWS |
| Auxiliam governança | Auxiliam transparência |
| Contêm informações do modelo | Contêm informações do serviço |

---

### A2I vs Model Monitor

| Amazon A2I | Model Monitor |
|------------|---------------|
| Revisão humana | Monitoramento automático |
| Human-in-the-Loop | Detecta mudanças no modelo |
| Atua durante decisões críticas | Atua após a implantação |

---

## 🧠 Conceitos importantes para prova

- Amazon Bedrock → IA generativa baseada em Foundation Models
- Amazon SageMaker → plataforma completa de Machine Learning
- SageMaker Clarify → viés, explicabilidade e avaliação de modelos
- Data Wrangler → preparação e balanceamento de dados
- SageMaker Experiments → gerenciamento de experimentos
- Model Monitor → monitora modelos em produção
- Amazon A2I → revisão humana (Human-in-the-Loop)
- Role Manager → gerenciamento de permissões
- Model Cards → documentação de modelos
- Model Dashboard → painel de governança
- AI Service Cards → documentação dos serviços de IA da AWS

---

## ⚠️ Pegadinhas comuns

- Bedrock não substitui o SageMaker
- Clarify identifica viés, mas não o corrige automaticamente
- Model Monitor não faz revisão humana
- A2I não monitora modelos
- AI Service Cards não são Model Cards
- Data Wrangler prepara os dados, mas não treina modelos
- SageMaker Experiments não monitora modelos em produção

---

## 🔁 Resumo rápido

| Serviço | Principal função |
|----------|------------------|
| Amazon Bedrock | IA generativa com Foundation Models |
| Amazon SageMaker | Plataforma de Machine Learning |
| SageMaker Clarify | Viés, explicabilidade e avaliação |
| Data Wrangler | Preparação e balanceamento de dados |
| SageMaker Experiments | Gerenciamento de experimentos |
| Model Monitor | Monitoramento de modelos |
| Amazon A2I | Revisão humana |
| Role Manager | Gerenciamento de permissões |
| Model Cards | Documentação de modelos |
| Model Dashboard | Governança |
| AI Service Cards | Transparência dos serviços da AWS |

---

## 📌 Status de aprendizado

- [ ] Sei diferenciar Amazon Bedrock e Amazon SageMaker
- [ ] Conheço a função do SageMaker Clarify
- [ ] Sei para que serve o Data Wrangler
- [ ] Entendo o papel do Model Monitor
- [ ] Sei quando utilizar o Amazon A2I
- [ ] Conheço Model Cards, Model Dashboard e AI Service Cards
