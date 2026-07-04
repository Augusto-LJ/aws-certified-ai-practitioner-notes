# 🤖 Agentes

Os **agentes** são componentes que ampliam as capacidades dos modelos de IA generativa, permitindo que eles interajam com sistemas externos, executem ações e automatizem fluxos de trabalho.

Enquanto um **LLM** é excelente para compreender linguagem natural e gerar respostas, ele normalmente **não possui acesso direto a bancos de dados, APIs ou sistemas corporativos**. Os agentes atuam justamente como essa ponte entre o modelo e o ambiente externo.

---

# 🎯 Objetivo dos agentes

Os agentes permitem que uma aplicação de IA generativa vá além de responder perguntas.

Com eles, a IA pode:

- Consultar sistemas internos
- Executar ações automaticamente
- Integrar diferentes serviços
- Automatizar processos complexos
- Coletar informações para melhorar continuamente o sistema

Em outras palavras, os agentes transformam um chatbot em um **assistente capaz de agir**, e não apenas conversar.

---

# ⚙️ Principais funções dos agentes

## 🔄 Operações intermediárias

Uma das principais funções dos agentes é atuar como intermediários entre o modelo de IA e os sistemas corporativos.

O LLM interpreta o pedido do usuário, mas quem realiza a comunicação com os sistemas da empresa é o agente.

### Exemplos de integração

- Bancos de dados
- Sistemas CRM
- Plataformas ERP
- Sistemas de atendimento
- APIs internas
- Ferramentas de gerenciamento de serviços

### Benefícios

- Integração segura com sistemas existentes
- Separação entre geração de linguagem e execução de ações
- Maior flexibilidade para expandir funcionalidades

---

## 🚀 Lançamento de ações

Após interpretar a intenção do usuário, o agente pode executar automaticamente diversas tarefas.

### Exemplos

- Alterar configurações de um serviço
- Atualizar plano contratado
- Solicitar segunda via de documentos
- Abrir chamados
- Processar transações
- Recuperar documentos
- Consultar informações em sistemas internos

Nesse cenário, o LLM identifica **o que deve ser feito**, enquanto o agente realiza **a execução da tarefa**.

---

## 📈 Integração de feedback

Os agentes também podem registrar informações sobre cada interação realizada.

Esses dados podem ser utilizados para:

- Avaliar o desempenho da IA
- Identificar erros recorrentes
- Atualizar bases de conhecimento
- Melhorar continuamente o sistema

O feedback coletado ajuda tanto na melhoria do modelo quanto da aplicação como um todo.

---

# 🏢 Caso de uso: AnyCompany

A **AnyCompany** deseja reduzir drasticamente o número de tickets de suporte utilizando IA generativa.

Para isso, além do chatbot e da arquitetura **RAG**, a empresa utiliza agentes responsáveis por executar tarefas específicas.

Cada agente possui uma responsabilidade bem definida:

<img width="944" height="589" alt="image" src="https://github.com/user-attachments/assets/79848aa4-a876-4134-9291-cc934e581d60" />

---

## 🤖 Agente 1 — Gerenciamento de planos

Responsável por executar alterações na conta do cliente.

### Exemplos

- Alterar plano telefônico
- Adicionar pacote de dados
- Solicitar novo aparelho
- Modificar configurações da conta

O usuário conversa naturalmente com o chatbot.

O LLM entende a solicitação.

O agente realiza a alteração diretamente nos sistemas da empresa.

---

## 🗂️ Agente 2 — Atualização da base de conhecimento

Esse agente utiliza as conversas realizadas com os clientes para enriquecer a base de conhecimento corporativa.

Pode realizar atividades como:

- Registrar novos problemas encontrados
- Atualizar perguntas frequentes (FAQ)
- Adicionar novos documentos
- Organizar informações relevantes

Esses novos dados podem posteriormente ser utilizados pelo sistema **RAG**, tornando as futuras respostas mais completas e precisas.

---

## ⭐ Agente 3 — Pesquisa de satisfação

Ao final do atendimento, esse agente envia automaticamente uma pesquisa de satisfação ao cliente.

Seu objetivo é medir indicadores importantes do negócio, como:

- Nível de satisfação
- Qualidade do atendimento
- Eficiência da IA
- Cumprimento das metas da empresa

Essas informações ajudam a empresa a acompanhar seus **KPIs** e identificar oportunidades de melhoria.

---

# 💡 Vantagens do uso de agentes

- Automatizam tarefas repetitivas
- Integram diversos sistemas corporativos
- Executam ações reais
- Melhoram a produtividade
- Reduzem trabalho manual
- Permitem aplicações muito mais inteligentes
- Coletam feedback para melhoria contínua

---

## 🔁 Comparações importantes

---

### LLM vs Agente

| LLM | Agente |
|------|---------|
| Compreende linguagem natural | Executa ações |
| Gera respostas | Interage com sistemas externos |
| Trabalha com texto | Trabalha com APIs, bancos de dados e serviços |
| Não altera sistemas sozinho | Pode modificar sistemas mediante autorização |

---

### RAG vs Agentes

| RAG | Agentes |
|------|----------|
| Recupera informações | Executa ações |
| Consulta base de conhecimento | Interage com sistemas externos |
| Melhora a qualidade das respostas | Automatiza processos |
| Fornece contexto ao LLM | Permite que o LLM realize tarefas |

---

## 🧠 Conceitos importantes para prova

- Agentes conectam o LLM aos sistemas corporativos.
- O LLM **decide o que deve ser feito**; o agente **executa a ação**.
- Agentes podem consultar bancos de dados, APIs e sistemas internos.
- Também podem coletar feedback para melhorar continuamente a aplicação.
- Em conjunto com o **RAG**, tornam aplicações de IA generativa muito mais úteis.
- Um sistema pode possuir **vários agentes**, cada um especializado em uma função.

---

## ⚠️ Pegadinhas comuns

- Agentes **não substituem** o LLM; eles complementam suas capacidades.
- Agentes **não são** bases de conhecimento.
- RAG recupera informações; agentes executam ações.
- Um LLM sozinho normalmente não altera sistemas corporativos.
- Agentes podem atuar tanto de forma automática quanto semiautomática.

---

## 🔁 Resumo rápido

- Agentes conectam modelos de IA aos sistemas da empresa.
- Permitem executar ações reais, além de responder perguntas.
- Podem consultar bancos de dados, APIs e serviços.
- Automatizam processos e integram diferentes sistemas.
- Também coletam feedback para melhorar continuamente a aplicação.
- No caso da AnyCompany, três agentes cuidam de alterações de planos, atualização da base de conhecimento e pesquisa de satisfação.

---

## 📌 Status de aprendizado

- [ ] Entendo o que são agentes em IA generativa
- [ ] Sei diferenciar agentes de LLMs
- [ ] Sei diferenciar agentes de RAG
- [ ] Entendo como agentes executam ações em sistemas externos
- [ ] Consigo explicar o papel dos agentes no caso da AnyCompany
