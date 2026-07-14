# 🏗️ Arquitetura e Casos de Uso do Amazon Q Business

O **Amazon Q Business** foi projetado para funcionar como um assistente corporativo inteligente, capaz de consultar informações da empresa, responder perguntas, gerar conteúdo e executar ações em aplicações empresariais.

Seu grande diferencial é combinar **IA generativa**, **RAG (Retrieval-Augmented Generation)**, **controle de acesso** e **integrações corporativas**, permitindo que usuários obtenham respostas contextualizadas de forma segura.

---

# 🏛️ Arquitetura do Amazon Q Business

A arquitetura do Amazon Q Business pode ser resumida no fluxo abaixo.

## 🔄 Fluxo de funcionamento

<img width="776" height="437" alt="image" src="https://github.com/user-attachments/assets/e3417f72-dc4f-4885-90e5-41e9ac88a773" />


---

### 1️⃣ Autenticação dos usuários

Antes de utilizar o serviço, o usuário é autenticado utilizando um **provedor de identidade compatível com SAML 2.0**.

Isso garante que apenas usuários autorizados tenham acesso à aplicação.

---

### 2️⃣ Consulta em linguagem natural

O usuário envia uma pergunta ou comando utilizando linguagem natural.

Exemplos:

- "Qual é nossa política de férias?"
- "Abra um chamado para o time de infraestrutura."
- "Resuma este documento."

---

### 3️⃣ Processamento pelo Amazon Q Business

O Amazon Q Business recebe a solicitação e utiliza diversos recursos para produzir a resposta.

Entre eles:

- 🤖 IA generativa
- 📚 Recuperação de informações (RAG)
- 🔒 Controles administrativos
- 🛡️ Guardrails
- 🔌 Plugins
- 🌐 APIs

---

### 4️⃣ Consulta às fontes de dados corporativas

Caso necessário, o serviço consulta documentos e sistemas internos utilizando seus conectores nativos.

Exemplos:

- Amazon S3
- SharePoint
- Google Drive
- Salesforce
- ServiceNow
- Jira

---

### 5️⃣ Resposta personalizada

Após recuperar as informações necessárias, o Amazon Q Business gera uma resposta baseada:

- No prompt enviado
- Nos documentos corporativos
- Nas permissões do usuário

Assim, cada usuário recebe apenas as informações às quais possui acesso.

---

### 6️⃣ Solicitação de ações

Além de responder perguntas, o usuário pode solicitar que determinadas ações sejam executadas.

Exemplos:

- Criar tickets
- Abrir incidentes
- Registrar chamados
- Criar casos de atendimento

Tudo isso sem precisar acessar diretamente a aplicação responsável.

---

### 7️⃣ Execução das ações

O Amazon Q Business utiliza seus plugins para executar essas ações em sistemas externos.

Exemplos:

- Jira
- Salesforce
- ServiceNow
- Zendesk

---

### 8️⃣ Conversa dentro das aplicações

Os usuários não precisam acessar uma interface separada.

O Amazon Q Business pode ser utilizado diretamente dentro das aplicações já utilizadas pela empresa.

---

### 9️⃣ Experiência integrada

Também é possível integrar o Amazon Q Business em ferramentas como:

- Slack
- Microsoft Teams

Assim, os usuários continuam trabalhando normalmente enquanto utilizam o assistente.

---

# ⚙️ Conceitos técnicos

Alguns componentes são fundamentais para o funcionamento do Amazon Q Business.

---

## 🆔 IAM Identity Center

O **IAM Identity Center** é utilizado para controlar quem pode utilizar a aplicação.

Ele funciona como uma camada de integração entre o Amazon Q Business e o provedor de identidade da organização.

É importante observar que ele **não substitui** o provedor de identidade existente.

Ele apenas facilita a autenticação e autorização dos usuários.

Após a configuração:

- Usuários podem ser atribuídos à aplicação.
- Grupos podem ser criados.
- Apenas usuários autorizados conseguem acessar o Amazon Q Business.

---

## 📚 Geração Aumentada por Recuperação (RAG)

Os LLMs possuem conhecimento adquirido durante seu treinamento.

Entretanto, eles não conhecem documentos internos da empresa.

Para resolver esse problema, o Amazon Q Business utiliza **RAG (Retrieval-Augmented Generation)**.

O funcionamento é simples:

1. O usuário faz uma pergunta.
2. O sistema procura documentos relacionados.
3. O conteúdo encontrado é enviado como contexto ao modelo.
4. O modelo gera uma resposta personalizada.

O Amazon Q Business gerencia automaticamente:

- Recuperação dos documentos
- Engenharia de prompts
- Embeddings vetoriais
- Contextualização

Os administradores podem configurar o comportamento da aplicação para:

- 📄 Responder apenas utilizando documentos corporativos.
- 🌎 Complementar a resposta com conhecimento geral quando necessário.

---

## 🔒 Controle de acesso aos dados

O Amazon Q Business respeita automaticamente as permissões existentes nos sistemas corporativos.

Ele pode integrar-se a provedores de identidade compatíveis com **SAML 2.0**, como:

- Okta
- Microsoft Entra ID
- Ping Identity

Dessa forma:

- Usuários autorizados acessam os documentos.
- Usuários sem permissão não conseguem visualizar essas informações.

---

## 🔄 Integração e sincronização dos dados

O serviço possui diversos conectores pré-construídos.

Esses conectores permitem sincronizar documentos corporativos de duas formas:

- 🔄 Sincronização completa
- ⚡ Sincronização incremental

Isso facilita manter a base de conhecimento sempre atualizada.

---

## 🔌 Plugins

Os plugins permitem que o Amazon Q Business execute ações em aplicações externas.

Exemplos:

- Criar tickets no Jira
- Abrir chamados no ServiceNow
- Criar casos no Salesforce
- Registrar solicitações no Zendesk

Os plugins ampliam significativamente as capacidades do assistente.

---

# 💼 Casos de uso

O Amazon Q Business pode ser utilizado em diversas áreas da empresa.

---

## ✍️ Criação acelerada de conteúdo

O serviço pode gerar conteúdos para diferentes departamentos.

Exemplos:

- Marketing
- Vendas
- RH
- Jurídico
- Pesquisa

### Exemplo

> "Escreva uma postagem para o blog anunciando este novo produto e gere três títulos para redes sociais."

O conteúdo será produzido considerando os documentos enviados e o conhecimento corporativo.

---

## 🔎 Pesquisa empresarial

O Amazon Q Business centraliza a pesquisa em diversos sistemas da organização.

O usuário não precisa mais procurar informações manualmente em vários locais.

### Exemplo

> "Onde estão as diretrizes mais recentes da marca?"

O serviço encontra o documento correto e informa sua localização.

Além disso, ele entende perguntas complementares.

Exemplo:

> "E onde encontro as versões antigas do logotipo?"

O contexto da conversa é mantido automaticamente.

---

## 📄 Geração de resumos

O Amazon Q Business pode resumir documentos extensos.

Exemplos:

- Relatórios
- Conversas no Slack
- Documentações
- Arquivos enviados

### Exemplo

> "Resuma os comentários dos clientes sobre nossa nova política de preços."

Isso permite compreender rapidamente grandes volumes de informação.

---

## 📊 Extração de informações

O serviço também pode analisar múltiplos documentos para extrair informações relevantes.

Exemplo:

> "Compare os relatórios de satisfação do cliente do primeiro e do segundo trimestre."

O Amazon Q Business identifica diferenças e gera insights para apoiar decisões de negócio.

---

# 🔐 Considerações importantes

---

## 🛡️ Uso dos dados do cliente

Os dados utilizados pelo Amazon Q Business **não são usados para treinar os modelos da AWS**.

Além disso, diversos dados são protegidos utilizando criptografia do **AWS KMS**, incluindo:

- Dados indexados
- Histórico das conversas
- Feedback dos usuários

---

## 💬 Histórico das conversas

O histórico do bate-papo é armazenado automaticamente por **30 dias**.

Os administradores podem excluir esse histórico quando necessário.

---

## 📁 Tipos de arquivos suportados

O Amazon Q Business suporta diversos formatos de documentos.

Exemplos:

- PDF
- DOCX
- CSV
- HTML
- JSON
- PPT

---

## 🤖 Escolha do LLM

O usuário **não escolhe diretamente** qual LLM será utilizado.

Internamente, a AWS utiliza diferentes modelos disponíveis no **Amazon Bedrock**.

---

## 🔌 Conectores personalizados

Além dos conectores nativos, também é possível criar conectores personalizados.

Para isso, utiliza-se o **Amazon Q SDK**.

Isso permite integrar praticamente qualquer sistema corporativo.

---

# ⚖️ RAG tradicional vs Amazon Q Business

| RAG tradicional | Amazon Q Business |
|-----------------|------------------|
| Desenvolvedor implementa todo o pipeline | Pipeline já gerenciado pela AWS |
| Engenharia de prompts manual | Automatizada |
| Gerenciamento dos embeddings | Gerenciado pelo serviço |
| Recuperação implementada manualmente | Recuperação integrada |
| Infraestrutura própria | Serviço totalmente gerenciado |

---

# 🧠 Conceitos importantes para prova

- O Amazon Q Business utiliza **RAG** para responder perguntas utilizando documentos corporativos.
- O IAM Identity Center é utilizado para controlar o acesso dos usuários.
- O serviço respeita as permissões existentes nas fontes de dados.
- Possui sincronização completa e incremental.
- Plugins permitem executar ações em aplicações externas.
- Pode ser integrado ao Slack e Microsoft Teams.
- O histórico das conversas permanece armazenado por um mês.
- Os dados dos clientes **não são utilizados para treinar os modelos**.
- O LLM utilizado não pode ser escolhido diretamente pelo usuário.

---

# ⚠️ Pegadinhas comuns

- O IAM Identity Center **não substitui** o provedor de identidade da empresa.
- O Amazon Q Business **não treina seus modelos utilizando dados do cliente**.
- O serviço gerencia automaticamente o pipeline de RAG.
- Plugins servem para executar ações, não apenas consultar dados.
- O usuário não escolhe qual modelo do Bedrock será utilizado.

---

# 🔁 Resumo rápido

- O Amazon Q Business autentica usuários utilizando SAML 2.0.
- Utiliza RAG para consultar documentos corporativos.
- Respeita automaticamente as permissões existentes.
- Possui conectores para dezenas de aplicações.
- Executa ações por meio de plugins.
- Pode ser utilizado diretamente em Slack e Microsoft Teams.
- Os dados do cliente são criptografados e não treinam os modelos da AWS.

---

# 📌 Status de aprendizado

- [ ] Entendo o fluxo da arquitetura do Amazon Q Business.
- [ ] Sei como funciona o uso de RAG no serviço.
- [ ] Entendo o papel do IAM Identity Center.
- [ ] Sei como o Amazon Q Business controla o acesso aos dados.
- [ ] Conheço os principais casos de uso.
- [ ] Sei quais informações são importantes para a certificação.
