# 🚀 Melhora do Desempenho de um Modelo de Base (FM)

<img width="910" height="105" alt="image" src="https://github.com/user-attachments/assets/f8daddcc-535e-46cb-92d1-995cc9f3c507" />

Após selecionar um **Modelo de Base (Foundation Model - FM)** adequado ao caso de uso, a próxima etapa é melhorar seu desempenho para atender melhor aos requisitos da aplicação.

Existem quatro principais abordagens:

- ✍️ Engenharia de Prompts
- 🔎 RAG (Retrieval-Augmented Generation)
- 🎯 Ajuste fino (Fine-tuning)
- 🤖 Agentes de automação

Cada uma possui diferentes níveis de custo, complexidade e personalização.

---

# ✍️ Engenharia de Prompts

A **Engenharia de Prompts (Prompt Engineering)** consiste em elaborar instruções capazes de orientar o modelo para produzir respostas mais úteis, precisas e alinhadas ao objetivo da aplicação.

É a forma **mais rápida e barata** de melhorar um modelo de IA generativa.

Em vez de modificar o modelo, modifica-se a forma como ele recebe as instruções.

---

## 🎯 Objetivos

- Melhorar a qualidade das respostas
- Reduzir ambiguidades
- Controlar o comportamento do modelo
- Minimizar respostas inadequadas
- Obter resultados mais consistentes

---

## 🔑 Aspectos importantes

### 📝 Design

Criar prompts claros, objetivos e ricos em contexto.

Exemplo:

❌ Explique IA.

✅ Explique IA generativa para um estudante universitário em até 5 parágrafos.

---

### ➕ Aprimoramento

Adicionar informações extras ao prompt.

Pode incluir:

- Exemplos
- Restrições
- Contexto
- Formato desejado

Quanto mais contexto relevante, maior tende a ser a qualidade da resposta.

---

### 🔄 Ajuste

Refinar continuamente os prompts.

O processo normalmente é iterativo:

1. Criar prompt
2. Avaliar resposta
3. Ajustar prompt
4. Testar novamente

---

### 📚 Agrupamento

Combinar múltiplos prompts ou estratégias para obter respostas mais robustas.

Exemplo:

- Um prompt gera ideias.
- Outro organiza.
- Outro revisa.

---

### ⛏️ Mineração de Prompts

Consiste em descobrir quais prompts produzem melhores resultados.

Pode envolver:

- Testes automáticos
- Bibliotecas de prompts
- Comparação entre diferentes versões

---

# 🛠️ Técnicas de Engenharia de Prompts

Existem diversas técnicas conhecidas.

As principais são:

- Zero-shot Prompting
- Few-shot Prompting
- Chain of Thought (CoT)
- Self-Consistency
- Tree of Thoughts (ToT)
- Retrieval-Augmented Generation (RAG)
- Automatic Reasoning and Tool Use (ART)
- ReAct Prompting

Neste curso, o foco está em **RAG**.

---

# 🔎 RAG (Retrieval-Augmented Generation)

A **Retrieval-Augmented Generation (RAG)** combina recuperação de informações com geração de texto.

Em vez de responder apenas com o conhecimento armazenado no modelo, a IA consulta uma base de conhecimento antes de gerar a resposta.

Isso torna as respostas:

- Mais atualizadas
- Mais precisas
- Mais contextualizadas

---

## 🏗️ Componentes da RAG

A RAG possui dois componentes principais.

### 📂 Sistema de Recuperação (Retriever)

Responsável por buscar informações relevantes em uma base de conhecimento.

As fontes podem incluir:

- Bancos de dados
- Documentos
- PDFs
- Sites
- Wikis corporativas
- FAQs

---

### 🧠 Modelo Generativo

Após recuperar as informações, o LLM utiliza esses dados para produzir uma resposta em linguagem natural.

Ele combina:

- Conhecimento recuperado
- Conhecimento aprendido durante o treinamento

---

## 🚀 Vantagens da RAG

- Respostas mais precisas
- Menor ocorrência de alucinações
- Utilização de informações atualizadas
- Não exige retreinamento do modelo
- Permite acesso a dados privados da organização

---

## 💼 Aplicações comerciais

### 💬 Chatbots inteligentes

Respondem utilizando bases de conhecimento corporativas.

---

### 📚 Bases de conhecimento

Expandem ou reorganizam informações existentes de forma mais acessível.

---

### 📝 Geração de conteúdo

Produzem:

- Relatórios
- Resumos
- Artigos
- Documentações

com apoio de informações reais.

---

## 🛠️ Exemplos no Amazon Bedrock

### 💬 Atendimento ao cliente

Base de conhecimento:

- Produtos
- FAQs
- Guias
- Solução de problemas

Aplicação:

Chatbot que consulta essas informações antes de responder.

---

### ⚖️ Pesquisa jurídica

Base:

- Leis
- Regulamentos
- Jurisprudência
- Pareceres

Aplicação:

Assistente jurídico inteligente.

---

### 🏥 Área médica

Base:

- Artigos científicos
- Diretrizes clínicas
- Doenças
- Tratamentos

Aplicação:

Assistentes virtuais especializados em saúde.

---

# 🎯 Ajuste Fino (Fine-Tuning)

O **Fine-Tuning** consiste em continuar o treinamento de um modelo pré-treinado utilizando dados específicos de uma tarefa ou domínio.

Assim, o modelo passa a responder melhor para um contexto específico.

---

## 🎯 Objetivos

- Especializar o modelo
- Melhorar a precisão
- Adaptar o modelo ao domínio da empresa
- Melhorar o desempenho em tarefas específicas

---

## 🛠️ Tipos de Fine-Tuning

### 📖 Ajuste fino por instruções

Ensina ao modelo como responder determinados tipos de instruções.

Exemplo:

Treinar um chatbot para responder sempre em linguagem jurídica.

---

### 👥 RLHF

**Reinforcement Learning from Human Feedback**

Utiliza avaliações humanas para ensinar quais respostas são melhores.

É uma das técnicas utilizadas por modelos modernos como o ChatGPT.

---

## ⚙️ Etapas do Fine-Tuning

### 1️⃣ Escolher um modelo pré-treinado

Seleciona-se um FM já treinado.

---

### 2️⃣ Preparar os dados

Coletam-se exemplos específicos da tarefa.

---

### 3️⃣ Adicionar componentes específicos

Caso necessário, adicionam-se camadas voltadas para a tarefa desejada.

---

### 4️⃣ Treinar novamente

O modelo aprende os novos padrões presentes no conjunto de dados.

---

### 5️⃣ Avaliar

O desempenho é testado.

Caso necessário, realiza-se novo ajuste.

---

## 💼 Exemplo

Um modelo geral pode ser ajustado utilizando:

- artigos médicos;
- protocolos clínicos;
- pesquisas científicas.

Após isso, torna-se muito mais eficiente para responder perguntas da área médica.

---

# 🏗️ Criando um Modelo do Zero

Em alguns casos, não existe um modelo pré-treinado adequado.

Nesse cenário pode ser criado um modelo completamente novo.

<img width="909" height="475" alt="image" src="https://github.com/user-attachments/assets/0466c885-f949-47c3-9281-bed499a8e225" />

---

## Etapas

1. Definir arquitetura
2. Coletar dados
3. Preparar dados
4. Inicializar pesos
5. Treinar o modelo
6. Avaliar
7. Repetir até atingir o desempenho desejado

---

## ✅ Vantagens

- Controle total
- Máxima personalização
- Melhor adaptação ao domínio

---

## ❌ Desvantagens

- Muito caro
- Exige enorme volume de dados
- Alto poder computacional
- Longo tempo de treinamento
- Necessidade de especialistas

---

# ⚖️ Trade-off entre custo e personalização

Existe uma relação direta entre custo e nível de personalização.

📈 Quanto maior a personalização, maior tende a ser:

- custo;
- tempo;
- complexidade.

A pirâmide apresentada no curso pode ser resumida assim:

```
Modelo criado do zero
        ▲
   Fine-Tuning
        ▲
RAG + Modelo Pré-treinado
        ▲
Modelo Pré-treinado
```

Quanto mais alto:

- maior personalização;
- maior custo;
- maior complexidade.

---

# 🤖 Agentes

Os **Agentes** são componentes capazes de executar tarefas automaticamente utilizando modelos de IA.

Eles dividem tarefas complexas em pequenas etapas e coordenam sua execução.

---

## Principais funções

### 🔄 Coordenação

Executam subtarefas na ordem correta.

---

### 📊 Relatórios

Produzem:

- logs
- métricas
- auditorias
- diagnósticos

---

### 📈 Escalabilidade

Executam diversas tarefas simultaneamente.

---

### 🔗 Integração

Comunicam-se com:

- APIs
- Bancos de dados
- Serviços externos
- Sistemas corporativos

---

## Exemplos no Amazon Bedrock

Os agentes podem automatizar:

- Provisionamento de infraestrutura
- Deploy de aplicações
- Backups
- Escalabilidade automática
- Monitoramento
- Configuração de recursos AWS

---

## 🔁 Comparações importantes

---

### Engenharia de Prompts vs Fine-Tuning

| Engenharia de Prompts | Fine-Tuning |
|----------------------|------------|
| Não altera o modelo | Altera o modelo |
| Rápido e barato | Mais caro e demorado |
| Usa apenas instruções | Exige novos dados para treinamento |
| Fácil de implementar | Requer treinamento adicional |

---

### RAG vs Fine-Tuning

| RAG | Fine-Tuning |
|------|------------|
| Consulta informações externas | Aprende novos padrões |
| Não modifica o modelo | Modifica os pesos do modelo |
| Ideal para conhecimento atualizado | Ideal para especialização |
| Reduz alucinações | Melhora comportamento e desempenho |

---

### Modelo Pré-treinado vs Modelo do Zero

| Modelo Pré-treinado | Modelo do Zero |
|--------------------|----------------|
| Menor custo | Alto custo |
| Implantação rápida | Longo tempo de desenvolvimento |
| Pouca personalização | Personalização total |
| Ideal para maioria dos casos | Usado apenas em casos muito específicos |

---

### RAG vs Modelo do Zero

| RAG | Modelo do Zero |
|------|----------------|
| Aproveita modelos existentes | Treina tudo do início |
| Baixo custo | Altíssimo custo |
| Mais simples | Muito complexo |
| Solução adotada na maioria das aplicações | Casos altamente especializados |

---

## 🧠 Conceitos importantes para prova

- Engenharia de Prompts é a forma mais rápida de melhorar um LLM.
- RAG combina recuperação de informações com geração de texto.
- RAG reduz alucinações sem alterar o modelo.
- Fine-Tuning adapta um modelo para um domínio específico.
- RLHF é uma forma de Fine-Tuning baseada em feedback humano.
- Criar um modelo do zero é a opção mais cara e complexa.
- Agentes automatizam tarefas compostas por múltiplas etapas.
- Na prática, a maioria das aplicações utiliza **Modelo Pré-treinado + RAG**.

---

## ⚠️ Pegadinhas comuns

- Engenharia de Prompts **não treina** o modelo.
- RAG **não altera** os pesos do modelo.
- Fine-Tuning **não cria** um novo modelo; apenas especializa um existente.
- RLHF é um tipo de ajuste fino baseado em avaliações humanas.
- Criar um modelo do zero raramente é a melhor opção.
- Mais personalização geralmente significa maior custo e maior complexidade.

---

## 🔁 Resumo rápido

- Melhorar um FM pode ser feito por Engenharia de Prompts, RAG, Fine-Tuning ou Agentes.
- Engenharia de Prompts é rápida e de baixo custo.
- RAG consulta bases de conhecimento antes de responder.
- Fine-Tuning especializa um modelo para tarefas específicas.
- Criar um modelo do zero oferece máxima personalização, porém exige muito investimento.
- Agentes automatizam processos complexos em múltiplas etapas.

---

## 📌 Status de aprendizado

- [ ] Entendo o que é Engenharia de Prompts
- [ ] Sei explicar como funciona a RAG
- [ ] Entendo a diferença entre RAG e Fine-Tuning
- [ ] Sei quando utilizar Fine-Tuning
- [ ] Entendo quando faz sentido criar um modelo do zero
- [ ] Sei o papel dos agentes em aplicações de IA generativa
