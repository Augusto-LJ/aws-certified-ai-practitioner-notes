# 🏢 Caso de Negócio — Otimizando um Modelo Base com RAG

Neste módulo, será utilizado um estudo de caso fictício da **AnyCompany**, uma empresa de telecomunicações, para demonstrar como a **Geração Aumentada de Recuperação (Retrieval-Augmented Generation — RAG)** pode ser utilizada para melhorar o desempenho de um modelo de IA generativa.

---

# 🏢 Cenário

A **AnyCompany** é uma empresa que fornece serviços de:

- 📞 Telefonia
- 🌐 Internet

Atualmente, quando um cliente possui algum problema, ele entra em contato com a central de suporte, principalmente por telefone.

Esse processo apresenta alguns problemas:

- Alto custo operacional
- Grande volume de atendimentos
- Baixa eficiência
- Tempo elevado para resolução de problemas

---

# 🎯 Objetivo da empresa

Para reduzir custos e melhorar a experiência do cliente, a AnyCompany iniciou uma migração para canais digitais.

A primeira iniciativa foi criar uma seção de **Perguntas Frequentes (FAQ)** no site para responder dúvidas comuns.

Apesar disso, a quantidade de solicitações de suporte continuou elevada.

Como próximo passo, a empresa decidiu desenvolver um **chatbot utilizando IA generativa**.

<img width="922" height="520" alt="image" src="https://github.com/user-attachments/assets/ae5007fb-8e26-4009-af01-7a038da9a3e6" />

---

# 🤖 Objetivos do chatbot

O chatbot deverá ser capaz de:

- Responder dúvidas frequentes
- Orientar clientes durante o atendimento
- Resolver problemas simples
- Executar algumas tarefas automaticamente

Exemplos de tarefas:

- 📱 Solicitar um novo aparelho
- 📶 Alterar o plano para mais dados 5G
- 👤 Atualizar informações da conta
- 🛠️ Auxiliar na resolução de problemas comuns

O objetivo é reduzir a necessidade de atendimento humano.

---

# 📈 Metas de negócio

A AnyCompany definiu dois indicadores principais (KPIs):

### 🎫 Redução dos tickets de suporte

Após a implantação do chatbot, a empresa espera reduzir em **70%** o número de tickets de suporte online.

---

### 😊 Satisfação do cliente

Após cada atendimento será aplicada uma pesquisa de satisfação.

Meta:

- Nota mínima de **4 de 5**

---

# 🧩 Desafio técnico

Para construir o chatbot, a empresa precisa escolher um **Foundation Model (FM)**.

Como o chatbot deverá compreender perguntas escritas em linguagem natural, o modelo escolhido precisa possuir capacidades de:

- Processamento de Linguagem Natural (NLP)
- Compreensão de contexto
- Geração de respostas em linguagem natural

Por isso, a escolha mais adequada é um **Large Language Model (LLM)**.

---

# ⚠️ Limitação dos LLMs

Embora um LLM possua amplo conhecimento geral, ele foi treinado principalmente com dados públicos.

Isso significa que ele **não conhece informações internas da AnyCompany**, como:

- Planos telefônicos atuais
- Procedimentos internos
- Políticas da empresa
- Histórico de suporte
- Dados específicos dos clientes

Sem acesso a essas informações, o chatbot pode produzir respostas incompletas, incorretas ou desatualizadas.

---

# 💡 Solução: utilizar RAG

Para fornecer respostas mais precisas, a empresa utilizará **Retrieval-Augmented Generation (RAG)**.

A ideia é complementar o conhecimento do LLM utilizando uma **base de conhecimento da própria empresa**.

Assim, antes de gerar uma resposta, o sistema busca informações relevantes e as fornece como contexto para o modelo.

---

# 📚 Fontes da base de conhecimento

A base de conhecimento poderá ser construída utilizando dados como:

- 💬 Registros de chats
- 🎫 Tickets de suporte anteriores
- 📞 Gravações de chamadas
- 📖 Documentação técnica
- ❓ Perguntas frequentes (FAQ)
- 📄 Procedimentos internos

Antes de serem utilizados, esses dados devem passar por etapas de:

- Coleta
- Limpeza
- Anonimização
- Organização

---

# 🤖 Automação de tarefas

Além de responder perguntas, o chatbot também deverá executar algumas ações automaticamente.

Exemplos:

- Alterar plano telefônico
- Solicitar envio de um novo aparelho
- Atualizar informações cadastrais
- Consultar informações da conta

Para isso, o chatbot precisará integrar-se aos sistemas internos da empresa e chamar funções específicas sempre que necessário.

Esse comportamento será realizado por meio de **agentes**, assunto abordado nas próximas páginas.

---

## 🔁 Comparações importantes

---

### FAQ tradicional vs Chatbot com RAG

| FAQ tradicional | Chatbot com RAG |
|----------------|-----------------|
| Conteúdo estático | Busca informações dinamicamente |
| Cliente precisa procurar a resposta | IA encontra a informação automaticamente |
| Pouca personalização | Respostas contextualizadas |
| Não executa ações | Pode integrar-se a sistemas e automatizar tarefas |

---

### LLM puro vs LLM com RAG

| LLM puro | LLM com RAG |
|----------|-------------|
| Usa apenas conhecimento do treinamento | Consulta uma base de conhecimento atualizada |
| Pode gerar respostas desatualizadas | Respostas mais precisas e contextualizadas |
| Não conhece informações internas da empresa | Utiliza dados específicos da organização |
| Maior chance de alucinações | Menor chance de alucinações relacionadas ao domínio |

---

## 🧠 Conceitos importantes para prova

- O objetivo da AnyCompany é reduzir custos e melhorar o atendimento ao cliente.
- O chatbot utilizará um **LLM** para compreender linguagem natural.
- Um LLM sozinho não possui conhecimento sobre informações internas da empresa.
- A **RAG** complementa o modelo utilizando uma base de conhecimento.
- Os dados da base devem ser coletados, limpos e anonimizados.
- O chatbot também poderá executar tarefas por meio de agentes.

---

## ⚠️ Pegadinhas comuns

- RAG **não retreina** o modelo; apenas fornece contexto adicional.
- O conhecimento interno da empresa **não faz parte** do treinamento original do LLM.
- FAQ e RAG não são a mesma coisa: a FAQ é uma fonte de informação, enquanto a RAG é uma técnica que recupera essas informações para o modelo.
- Para automatizar ações (como alterar um plano), o chatbot precisa integrar-se aos sistemas da empresa, normalmente utilizando agentes.

---

## 🔁 Resumo rápido

- A AnyCompany deseja reduzir o volume de atendimentos humanos.
- O chatbot será baseado em um LLM.
- Como o LLM não conhece dados internos, será utilizada a técnica **RAG**.
- A RAG consulta uma base de conhecimento antes da geração da resposta.
- O chatbot também poderá executar ações integrando-se aos sistemas da empresa.

---

## 📌 Status de aprendizado

- [ ] Entendo o problema enfrentado pela AnyCompany
- [ ] Sei por que um LLM foi escolhido para o chatbot
- [ ] Entendo por que um LLM puro não é suficiente
- [ ] Sei como a RAG resolve esse problema
- [ ] Entendo por que o chatbot precisa integrar-se aos sistemas internos
