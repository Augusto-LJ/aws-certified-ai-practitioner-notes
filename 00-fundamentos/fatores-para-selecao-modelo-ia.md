# 🎯 Seleção de Modelos de IA Generativa

## 📌 O que é

Ao utilizar IA generativa, é importante escolher o modelo mais adequado para o caso de uso.

📌 Não existe um modelo melhor para tudo.

Cada modelo possui:
- Capacidades diferentes
- Custos diferentes
- Requisitos diferentes
- Casos de uso específicos

---

## 🎯 Quando analisar

Sempre que for necessário:

- Criar uma aplicação com IA generativa
- Escolher um Foundation Model (FM)
- Comparar modelos disponíveis no Amazon Bedrock
- Avaliar custo vs desempenho

---

## ⚙️ Principais fatores de decisão

### 🧠 Tipo de modelo (Model Type)

O primeiro passo é identificar a tarefa que será executada.

- Ex:
  - Geração de texto
  - Geração de imagens
  - Chatbots
  - Tradução
  - Resumo
  - Geração de código

📌 Alguns modelos são especializados em determinadas tarefas.

---

### 🚀 Requisitos de desempenho (Performance Requirements)

Avalie:

- Acurácia (Accuracy)
- Confiabilidade (Reliability)
- Consistência das respostas
- Latência (Latency)

📌 O modelo deve atender aos requisitos do negócio.

---

### ⚙️ Capacidades (Capabilities)

Cada modelo possui capacidades diferentes.

- Ex:
  - Texto
  - Código
  - Imagem
  - Embeddings
  - Busca semântica
  - Multimodalidade

📌 Nem todo modelo suporta todas as funcionalidades.

---

### 🏗️ Restrições (Constraints)

Considere limitações relacionadas a:

- CPU
- GPU
- Memória
- Dados disponíveis
- Ambiente de implantação

- Ex:
  - Cloud
  - On-premises

📌 Alguns modelos exigem muito mais recursos computacionais.

---

### ⚖️ Conformidade (Compliance)

Avalie requisitos relacionados a:

- Privacidade
- Segurança
- Regulamentações
- Governança

Também considere riscos como:

- Bias
- Toxicity
- Hallucinations

📌 Especialmente importante em:
- Saúde
- Finanças
- Jurídico

---

### 💰 Custo (Cost)

Avalie:

- Implantação
- Inferência
- Treinamento
- Armazenamento
- Hardware

📌 Regra geral:

| Modelos maiores | Modelos menores |
|----------------|----------------|
| Mais precisos | Menos precisos |
| Mais caros | Mais baratos |
| Mais lentos | Mais rápidos |
| Menos opções de implantação | Mais flexíveis |

---

## 🏢 Exemplos de Foundation Models

### 🤖 Amazon Titan

#### Capacidades

- Resumo
- Classificação
- Perguntas e respostas
- Embeddings
- Busca semântica

#### Casos de uso

- Atendimento ao cliente
- Pesquisa corporativa
- Aplicações de busca

---

### 🧠 Claude (Anthropic)

#### Capacidades

- Geração de conteúdo
- Resumo
- Tradução
- Perguntas e respostas
- Geração de código

#### Casos de uso

- Assistentes virtuais
- Desenvolvimento de software
- Análise de documentos

---

### 🦙 Llama (Meta)

#### Capacidades

- Chat
- Resumo
- Análise de sentimento
- Geração de texto

#### Casos de uso

- Chatbots
- Atendimento ao cliente

---

### ✍️ Command (Cohere)

#### Capacidades

- Geração de texto
- Perguntas e respostas
- Resumo
- Extração de informações

#### Casos de uso

- Atendimento ao cliente
- Descrições de produtos

---

### 🎨 Stable Diffusion (Stability AI)

#### Capacidades

- Geração de imagens
- Edição de imagens
- Aprimoramento visual

#### Casos de uso

- Marketing
- Publicidade
- Jogos
- Design

---

### 📚 Jurassic-2 (AI21 Labs)

#### Capacidades

- Geração de texto
- Resumo
- Parafraseamento
- Chat

#### Casos de uso

- Documentação
- Resumos corporativos

---

## 🧩 Considerações responsáveis na seleção de modelos de IA

A escolha de um modelo é uma das decisões mais importantes no desenvolvimento de sistemas de IA. A seleção correta influencia diretamente:

- Desempenho da solução
- Experiência do usuário
- Tempo de lançamento no mercado (Time to Market)
- Custos operacionais
- Escalabilidade
- Conformidade regulatória
- Sustentabilidade
- Aplicação dos princípios de IA Responsável (Responsible AI)

A AWS disponibiliza ferramentas como:

- Amazon Bedrock Model Evaluation
- Amazon SageMaker Clarify

Essas ferramentas ajudam a avaliar modelos quanto a:

- Precisão (Accuracy)
- Robustez (Robustness)
- Toxicidade (Toxicity)
- Viés (Bias)
- IA Responsável (Responsible AI)

---

### 🎯 Definir claramente o caso de uso (Define the Use Case Narrowly)

Antes de selecionar um modelo, é fundamental definir claramente o problema que a aplicação deve resolver.

O mesmo modelo pode ser adequado para determinados cenários e inadequado para outros.

#### Exemplo: IA tradicional

Reconhecimento facial (Facial Recognition) é uma tecnologia, não um caso de uso.

Casos de uso possíveis:

- Busca de pessoas desaparecidas
- Reconhecimento de celebridades
- Supervisão virtual
- Controle de acesso

Cada cenário exige ajustes, métricas e níveis de precisão diferentes.

#### Exemplo: IA generativa

Uma aplicação de e-commerce pode utilizar IA para diferentes objetivos.

##### Catalogar produtos

Características:

- Público amplo
- Linguagem neutra
- Foco em precisão das informações

Prioridades:

- Clareza (Clarity)
- Neutralidade (Neutrality)
- Integridade (Completeness)
- Veracidade (Truthfulness)

##### Persuadir clientes a comprar

Características:

- Público específico
- Comunicação direcionada

Prioridades:

- Personalização (Personalization)
- Persuasão (Persuasion)
- Engajamento (Engagement)

Riscos adicionais:

- Viés (Bias)
- Toxicidade (Toxicity)
- Informações incorretas

---

### ⚡ Seleção baseada em desempenho (Performance-Based Selection)

Ao selecionar um modelo, avalie seu desempenho para o caso de uso específico.

#### Principais fatores de desempenho

- Nível de personalização (Customization)
- Tamanho do modelo (Model Size)
- Opções de inferência (Inference Options)
- Contratos de licenciamento (Licensing Agreements)
- Janela de contexto (Context Window)
- Latência (Latency)

#### Avaliação baseada em datasets

Um erro comum é considerar que um modelo é simplesmente "bom" ou "ruim".

O desempenho depende da combinação entre:

- Modelo
- Conjunto de dados utilizado

O mesmo modelo pode:

- Ter excelente desempenho em um dataset
- Ter desempenho mediano em outro
- Ter desempenho ruim em um terceiro

Por isso, os testes devem utilizar dados representativos do cenário real.

---

### 📊 Avaliação de modelos (Model Evaluation)

A avaliação deve ocorrer antes da implantação em produção.

#### Amazon Bedrock Model Evaluation

Permite:

- Avaliar modelos de base (Foundation Models - FMs)
- Comparar diferentes modelos
- Selecionar o modelo mais adequado

Métricas avaliadas:

- Precisão (Accuracy)
- Robustez (Robustness)
- Toxicidade (Toxicity)

Tipos de avaliação:

- Automática
- Humana

#### Amazon SageMaker Clarify

Permite:

- Avaliar Foundation Models
- Detectar viés
- Avaliar robustez
- Medir toxicidade
- Realizar avaliações humanas quando necessário

---

### 🤝 Considerações sobre agência responsável (Responsible Agency)

A IA Responsável busca garantir que os sistemas de IA tomem decisões alinhadas aos valores humanos.

#### Alinhamento de valores (Value Alignment)

O sistema deve atuar de acordo com:

- Valores humanos
- Princípios éticos
- Objetivos organizacionais

#### Raciocínio responsável (Responsible Reasoning)

O sistema deve ser capaz de:

- Avaliar consequências
- Considerar aspectos éticos
- Aplicar regras adequadas ao contexto

#### Nível adequado de autonomia (Appropriate Level of Autonomy)

Aplicações de IA devem possuir:

- Supervisão humana
- Limites operacionais claros
- Mecanismos de intervenção humana

Especialmente em sistemas críticos.

#### Transparência e responsabilidade (Transparency and Accountability)

Os usuários devem conseguir compreender:

- Como o sistema toma decisões
- Quais dados influenciam os resultados
- Quais são as limitações do modelo

---

### 🌱 Sustentabilidade (Sustainability)

A sustentabilidade deve ser considerada durante a seleção do modelo.

Modelos maiores normalmente exigem:

- Mais energia
- Mais processamento
- Mais infraestrutura

Isso aumenta:

- Custos
- Consumo energético
- Impacto ambiental

#### Aspectos importantes

- Eficiência energética (Energy Efficiency)
- Uso de energia renovável (Renewable Energy)
- Pegada de carbono (Carbon Footprint)

---

### 🌍 Considerações ambientais (Environmental Considerations)

#### Consumo de energia (Energy Consumption)

##### Desafio

Treinar e executar grandes modelos pode consumir grandes quantidades de energia.

##### Mitigação

- Otimizar eficiência energética
- Utilizar fontes renováveis
- Avaliar a pegada de carbono da solução

#### Utilização de recursos (Resource Utilization)

##### Desafio

Modelos avançados exigem:

- GPUs
- TPUs
- Datacenters

A fabricação e descarte desses recursos também geram impactos ambientais.

##### Mitigação

- Reutilização de hardware
- Reciclagem
- Redução de desperdício eletrônico

#### Avaliação de impacto ambiental (Environmental Impact Assessment)

Antes da implantação, devem ser avaliados:

- Consumo de energia
- Uso de recursos
- Possíveis impactos ambientais indiretos

---

### 💰 Considerações econômicas (Economic Considerations)

Além dos fatores técnicos, a seleção do modelo deve considerar impactos econômicos.

#### Benefícios potenciais

- Automação de tarefas
- Redução de custos operacionais
- Aumento da produtividade
- Escalabilidade

#### Possíveis desafios

- Custos de treinamento
- Custos de inferência
- Necessidade de infraestrutura especializada
- Impactos no mercado de trabalho

A escolha ideal busca equilibrar:

- Custo (Cost)
- Desempenho (Performance)
- Escalabilidade (Scalability)
- Sustentabilidade (Sustainability)
- Responsabilidade (Responsible AI)

---

### 📝 Resumo para a prova

Ao selecionar um modelo de IA generativa, considere:

- Caso de uso (Use Case)
- Desempenho (Performance)
- Capacidades (Capabilities)
- Restrições (Constraints)
- Conformidade (Compliance)
- Custos (Cost)
- Sustentabilidade (Sustainability)
- Transparência (Transparency)
- Imparcialidade (Fairness)
- Privacidade e segurança (Privacy and Security)
- Nível de autonomia (Autonomy)

#### Ferramentas AWS cobradas na prova

- Amazon Bedrock Model Evaluation
- Amazon SageMaker Clarify

Essas ferramentas ajudam a avaliar:

- Precisão (Accuracy)
- Robustez (Robustness)
- Toxicidade (Toxicity)
- Viés (Bias)
- IA Responsável (Responsible AI)

## 🔁 Comparações importantes

### Claude vs Llama

| Claude | Llama |
|----------|----------|
| Forte em análise e geração de conteúdo | Forte em conversação |
| Muito usado para documentos | Muito usado para chatbots |

---

### Titan vs Claude

| Titan | Claude |
|--------|---------|
| Modelo da AWS | Modelo da Anthropic |
| Possui embeddings | Forte em geração de texto e código |

---

### Texto vs Imagem

| Modelos de texto | Modelos de imagem |
|-----------------|------------------|
| Claude | Stable Diffusion |
| Titan Text | Stable Diffusion |
| Llama | Stable Diffusion |

---

## 🧠 Conceitos importantes para prova

- Não existe um único modelo ideal
- A escolha depende do caso de uso
- Avaliar:
  - Capacidades
  - Custo
  - Desempenho
  - Restrições
  - Conformidade
- Foundation Models possuem características diferentes
- Amazon Bedrock permite acesso a múltiplos modelos através de uma única API

---

## ⚠️ Pegadinhas comuns

- Modelo maior não significa melhor para todos os cenários
- Modelo mais caro não significa melhor custo-benefício
- Nem todo modelo gera imagens
- Nem todo modelo gera código
- A escolha do modelo depende dos requisitos da aplicação

---

## 🔁 Resumo rápido

- Escolha o modelo com base no caso de uso
- Considere:
  - Tipo de tarefa
  - Desempenho
  - Capacidades
  - Restrições
  - Conformidade
  - Custo
- Amazon Bedrock oferece diversos Foundation Models
- Diferentes modelos são otimizados para diferentes tarefas

---

## 📌 Status de aprendizado

- [ ] Sei quais fatores analisar ao escolher um modelo
- [ ] Entendo a diferença entre capacidades e desempenho
- [ ] Sei quando considerar conformidade
- [ ] Entendo o impacto do custo na escolha do modelo
- [ ] Conheço os principais Foundation Models disponíveis no Bedrock
