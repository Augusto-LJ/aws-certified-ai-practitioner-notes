# 🪨 Amazon Bedrock

O **Amazon Bedrock** é um serviço **serverless e totalmente gerenciado** da AWS que permite criar aplicações de **IA generativa** utilizando **Foundation Models (FMs)** de diversos provedores por meio de **uma única API**.

O grande objetivo do Bedrock é permitir que empresas utilizem IA generativa **sem precisar treinar modelos, gerenciar infraestrutura ou possuir profundo conhecimento em Machine Learning**.
---

# 🎯 Objetivos do Amazon Bedrock

O Bedrock foi criado para facilitar o desenvolvimento de aplicações de IA generativa.

Ele permite:

- 🤖 Utilizar Foundation Models prontos
- ⚙️ Acessar modelos através de uma API unificada
- 🔒 Manter os dados privados
- 🎨 Personalizar modelos para o domínio da empresa
- 📈 Escalar automaticamente sem infraestrutura

---

# ❓ Quais problemas o Bedrock resolve?

Antes do Bedrock, utilizar modelos generativos exigia:

- Gerenciar infraestrutura de GPU
- Implantar modelos manualmente
- Integrar diferentes APIs de cada provedor
- Conhecimento avançado em Machine Learning

Com o Bedrock, tudo isso é abstraído.

O desenvolvedor apenas escolhe o modelo e envia o prompt.

---

# ⚙️ Como funciona

O fluxo básico é bastante simples:

1. Escolher um Foundation Model
2. Enviar um prompt
3. O Bedrock executa a inferência
4. Receber a resposta gerada

Tudo acontece através de uma **API única**, independentemente do provedor do modelo.

---

# 🧠 Foundation Models (FMs)

Os **Foundation Models** são modelos de IA treinados em grandes volumes de dados e capazes de realizar diversas tarefas.

Exemplos:

- Geração de texto
- Resumos
- Tradução
- Geração de código
- Geração de imagens
- Embeddings

Diferentemente dos modelos tradicionais de Machine Learning, eles são **genéricos** e podem ser adaptados para inúmeros casos de uso.

---

# 🤖 Modelos disponíveis

O Amazon Bedrock reúne modelos de diversos provedores em uma única plataforma.

## 🟠 Amazon Nova

A família **Amazon Nova** é composta pelos modelos mais recentes da AWS.

| Modelo | Principal característica |
|---------|-------------------------|
| Nova Micro | Texto com baixa latência e baixo custo |
| Nova Lite | Multimodal econômico (texto, imagem e vídeo) |
| Nova Pro | Multimodal equilibrado entre custo, velocidade e qualidade |
| Nova Premier | Modelo mais avançado para tarefas complexas |
| Nova Canvas | Geração e edição de imagens |
| Nova Reel | Geração de vídeos |
| Nova Sonic | Conversação por voz em tempo real |

> 📌 Para a prova, basta saber que a família **Nova** oferece modelos especializados para texto, multimodalidade, imagens, vídeos e voz.

---

## 🟡 Amazon Titan

Outra família de modelos da AWS disponível no Bedrock.

É utilizada em diversos cenários como:

- Geração de texto
- Embeddings
- IA generativa empresarial

---

## 🌎 Outros provedores

Além dos modelos da AWS, o Bedrock oferece acesso a modelos de diversos fornecedores, como:

- Anthropic (Claude)
- AI21 Labs
- Cohere
- Meta
- Stability AI

Todos são utilizados através da **mesma API**.

> 📌 Grande vantagem: trocar de modelo não exige aprender uma API diferente.

---

# 🎨 Personalização dos modelos

O Bedrock oferece duas formas principais de personalizar um modelo.

## 🏋️ Fine-tuning

Treina o modelo utilizando dados da empresa.

Ideal quando se deseja adaptar:

- Estilo de escrita
- Terminologia
- Conhecimento específico

---

## 📚 RAG (Retrieval-Augmented Generation)

Em vez de alterar o modelo, o RAG consulta informações externas durante a geração da resposta.

Exemplos:

- Documentação da empresa
- PDFs
- Wikis
- Bases internas

> 📌 RAG não modifica o modelo.

---

# 🧩 Conceitos técnicos importantes

## 📝 Tokens

Os modelos trabalham com **tokens**, e não diretamente com palavras.

O custo normalmente é calculado pela quantidade de:

- Tokens de entrada (Input)
- Tokens de saída (Output)

Cada modelo possui um limite máximo de tokens.

---

## ✍️ Engenharia de Prompt (Prompt Engineering)

Consiste em escrever prompts de forma eficiente para obter melhores respostas.

Boas práticas:

- Ser específico
- Informar contexto
- Definir formato da resposta
- Dar exemplos (Few-shot)

---

## ⚙️ Parâmetros de inferência

Controlam o comportamento do modelo.

### 🌡️ Temperatura (Temperature)

Controla a criatividade.

- Baixa → respostas previsíveis
- Alta → respostas mais criativas

---

### 🎯 Top-p

Limita a seleção de palavras às opções mais prováveis.

Ajuda a controlar criatividade e consistência.

---

### 📏 Max Tokens

Define o tamanho máximo da resposta.

Também influencia o custo.

---

# 📚 RAG (Retrieval-Augmented Generation)

O Bedrock possui suporte nativo para RAG.

Fluxo simplificado:

1. Usuário envia uma pergunta
2. O sistema busca documentos relevantes
3. Essas informações são adicionadas ao prompt
4. O modelo gera uma resposta baseada nesse contexto

> 📌 Ideal quando os dados mudam frequentemente.

---

# 📊 Avaliação de modelos

O Bedrock fornece ferramentas para comparar diferentes modelos.

Permite avaliar critérios como:

- Precisão
- Relevância
- Segurança
- Qualidade das respostas

Isso facilita escolher o modelo mais adequado para cada aplicação.

---

# 🔄 Flows (Fluxos)

Os **Flows** permitem criar fluxos de IA utilizando uma interface visual (low-code/no-code).

Um fluxo pode combinar:

- Foundation Models
- Bases de conhecimento
- Funções personalizadas
- Lógicas condicionais

Exemplo:

Documento → Resumo → Geração de resposta.

---

# 🤖 Agents for Amazon Bedrock

Os agentes permitem criar aplicações capazes de executar tarefas automaticamente.

Eles podem:

- Interpretar solicitações
- Consultar bases de conhecimento
- Chamar APIs
- Executar funções
- Manter contexto da conversa

Exemplo:

Um agente de e-commerce pode:

- Consultar pedidos
- Processar devoluções
- Verificar estoque
- Abrir chamados

---

# 🔐 Segurança

O Amazon Bedrock foi desenvolvido para ambientes corporativos.

Principais recursos:

- IAM
- AWS KMS
- AWS CloudTrail
- VPC Endpoints
- AWS PrivateLink

Além disso:

✅ Os dados enviados **não são utilizados para treinar os modelos**.

---

# 🛡️ Governança e Guardrails

Os **Guardrails** ajudam a controlar o comportamento da IA.

Permitem:

- Bloquear conteúdos inadequados
- Filtrar respostas
- Restringir temas
- Aplicar políticas corporativas

Também auxiliam no desenvolvimento responsável de aplicações de IA.

---

# ⭐ Principais recursos

## 🌎 API unificada

Um único padrão de integração para diversos Foundation Models.

---

## 🎨 Personalização

Suporte para:

- Fine-tuning
- RAG

---

## 🤖 Framework de agentes

Permite criar agentes inteligentes que utilizam:

- Ferramentas
- APIs
- Bases de conhecimento
- Fluxos de trabalho

---

## ☁️ Arquitetura Serverless

Não é necessário:

- Provisionar servidores
- Gerenciar clusters
- Planejar escalabilidade

O Bedrock escala automaticamente.

---

## 🔒 Segurança empresarial

Inclui:

- IAM
- PrivateLink
- Criptografia
- Conformidade AWS
- Dados privados

---

## ⚖️ IA Responsável

O Bedrock oferece ferramentas para:

- Avaliação de modelos
- Guardrails
- Filtragem de conteúdo
- Monitoramento

---

# 💼 Casos de uso

## ✍️ Geração de conteúdo

Exemplos:

- Blogs
- E-mails
- Marketing
- Redes sociais
- Descrições de produtos

---

## 💬 Atendimento ao cliente

Chatbots capazes de:

- Responder perguntas
- Consultar documentos
- Utilizar bases internas
- Automatizar atendimento

---

## 📊 Análise de documentos

Permite:

- Resumir documentos
- Extrair informações
- Comparar contratos
- Responder perguntas sobre documentos

---

## 💻 Assistência ao desenvolvimento

Pode auxiliar em:

- Geração de código
- Explicação de código
- Documentação
- Correção de erros

---

## 🏢 Gestão do conhecimento

Criação de assistentes internos utilizando RAG para consultar:

- Wikis
- PDFs
- Documentação
- Bases corporativas

---

# 🔁 Comparações importantes

---

## Amazon Bedrock vs SageMaker

| Bedrock | SageMaker |
|--------|----------|
| Usa modelos prontos | Cria e treina modelos |
| Serverless | Gerencia infraestrutura |
| Foco em IA generativa | Foco em Machine Learning |
| Mais simples | Mais flexível |

---

## Bedrock vs AI Services

| Bedrock | AI Services |
|--------|-------------|
| IA Generativa | IA tradicional |
| Baseado em prompts | APIs específicas |
| Foundation Models | Modelos especializados |

---

## Fine-tuning vs RAG

| Fine-tuning | RAG |
|-------------|-----|
| Altera o modelo | Não altera o modelo |
| Requer treinamento | Consulta dados externos |
| Bom para comportamento | Bom para conhecimento atualizado |
| Mais caro | Mais barato |

---

## Flows vs Agents

| Flows | Agents |
|--------|---------|
| Orquestram processos | Executam tarefas |
| Fluxos visuais | Assistentes inteligentes |
| Sequência de etapas | Tomam decisões e utilizam ferramentas |

---

# 🧠 Conceitos importantes para prova

- Amazon Bedrock é um serviço **serverless**.
- Fornece acesso a diversos **Foundation Models**.
- Utiliza **uma única API** para todos os provedores.
- Não exige gerenciamento de infraestrutura.
- Suporta **Fine-tuning** e **RAG**.
- Os dados do cliente **não são utilizados para treinar os modelos**.
- Possui **Agents**, **Flows** e **Guardrails**.
- Integra-se facilmente com outros serviços da AWS.

---

# ⚠️ Pegadinhas comuns

- Bedrock **não serve para treinar modelos do zero**.
- Fine-tuning e RAG são técnicas diferentes.
- RAG adiciona contexto; **não modifica o modelo**.
- O Bedrock oferece modelos de diversos fornecedores, não apenas da AWS.
- Guardrails não aumentam a inteligência do modelo; eles controlam seu comportamento.
- O Bedrock é totalmente gerenciado e serverless.

---

# 🔁 Resumo rápido

- Bedrock é a plataforma de IA generativa da AWS.
- Fornece acesso a vários Foundation Models por uma API única.
- É serverless e totalmente gerenciado.
- Permite personalização com Fine-tuning e RAG.
- Inclui Agents, Flows e Guardrails.
- Possui forte foco em segurança, governança e IA responsável.
- É um dos serviços mais importantes para a certificação AWS AI Practitioner.

---

# 📌 Status de aprendizado

- [ ] Entendo o que é o Amazon Bedrock
- [ ] Sei o que são Foundation Models
- [ ] Sei diferenciar Fine-tuning e RAG
- [ ] Entendo o funcionamento de Tokens e Prompt Engineering
- [ ] Sei o papel dos parâmetros de inferência
- [ ] Entendo o que são Flows e Agents
- [ ] Sei como funcionam Guardrails
- [ ] Conheço os principais casos de uso do Bedrock
- [ ] Sei as principais diferenças entre Bedrock e SageMaker
