# 🎯 Ajuste Fino (Fine-tuning)

Os **Modelos de Base (Foundation Models - FMs)** possuem conhecimento geral sobre diversos assuntos, mas normalmente precisam ser adaptados para atender às necessidades específicas de uma empresa ou aplicação.

O **ajuste fino (Fine-tuning)** é o processo de continuar o treinamento de um modelo pré-treinado utilizando um conjunto de dados específico, permitindo que ele se torne mais especializado em determinado domínio ou tarefa.

Em vez de criar um modelo do zero, aproveita-se todo o conhecimento já adquirido pelo modelo e o adapta para um novo contexto.

---

# 🎯 Por que fazer ajuste fino?

O ajuste fino permite especializar um modelo para resolver problemas específicos de forma mais eficiente.

## 📌 Aumentar a especificidade

O modelo aprende características próprias de um domínio.

Exemplos:

- Medicina
- Direito
- Atendimento ao cliente
- Moda
- Mercado financeiro

Assim, as respostas tornam-se mais adequadas ao contexto.

---

## 🎯 Melhorar a precisão

Treinar o modelo com dados específicos reduz erros causados pelo conhecimento excessivamente genérico.

Como resultado:

- Respostas mais corretas
- Melhor entendimento do contexto
- Maior confiabilidade

---

## ⚖️ Reduzir vieses

O ajuste fino também pode ser utilizado para minimizar vieses presentes durante o pré-treinamento.

Isso torna o modelo:

- Mais justo
- Mais equilibrado
- Mais adequado ao contexto da aplicação

---

## ⚡ Aumentar a eficiência

Ao especializar o modelo, é possível reduzir respostas desnecessárias e aumentar sua eficiência para tarefas específicas.

Benefícios:

- Respostas mais objetivas
- Melhor desempenho
- Maior produtividade

---

# 🔧 Principais abordagens de ajuste fino

Existem diferentes técnicas para adaptar um modelo de base.

---

## 📝 Ajuste de instruções (Instruction Tuning)

Nessa abordagem, o modelo é treinado utilizando exemplos compostos por:

- Um prompt (instrução)
- A resposta desejada

O objetivo é ensinar o modelo a seguir instruções de maneira mais precisa.

### Exemplos

Prompt:

> Resuma este texto em uma frase.

Resposta esperada:

> Resumo do texto.

---

### Casos de uso

- Chatbots
- Assistentes virtuais
- Copilotos de programação
- Sistemas de perguntas e respostas

---

## 👥 RLHF (Reinforcement Learning from Human Feedback)

O **Aprendizado por Reforço com Feedback Humano (RLHF)** utiliza avaliações feitas por pessoas para melhorar continuamente o comportamento do modelo.

O processo ocorre, de forma simplificada, da seguinte maneira:

1. O modelo gera respostas.
2. Pessoas avaliam essas respostas.
3. Um modelo de recompensa aprende essas preferências.
4. O modelo passa a produzir respostas mais alinhadas às expectativas humanas.

O RLHF pode ser utilizado tanto durante o pré-treinamento quanto no ajuste fino.

### Benefícios

- Respostas mais úteis
- Menor toxicidade
- Melhor alinhamento com valores humanos
- Melhor experiência do usuário

---

## 🏢 Adaptação para domínios específicos

Nessa abordagem, o modelo é ajustado utilizando documentos especializados de um determinado setor.

### Exemplos

- Artigos médicos
- Documentos jurídicos
- Relatórios financeiros
- Base de conhecimento corporativa

O objetivo é aumentar a precisão em tarefas específicas daquele domínio.

---

## 🔄 Aprendizado por transferência (Transfer Learning)

O aprendizado por transferência reutiliza o conhecimento já adquirido por um modelo para acelerar o aprendizado em uma nova tarefa.

Em vez de começar do zero, utiliza-se um modelo pré-treinado como ponto de partida.

### Benefícios

- Menor custo
- Menor tempo de treinamento
- Menor necessidade de dados

---

## 🔁 Pré-treinamento contínuo (Continued Pre-training)

Consiste em continuar alimentando o modelo com novos dados ao longo do tempo.

Essa técnica mantém o modelo atualizado com:

- Novas pesquisas
- Novos acontecimentos
- Mudanças no vocabulário
- Tendências recentes

É especialmente útil quando o domínio evolui rapidamente.

---

# 📚 Preparação de dados no pré-treinamento

Durante o pré-treinamento, o objetivo é ensinar conhecimento geral ao modelo.

Os dados utilizados possuem algumas características importantes.

## 🌎 Cobertura abrangente

O conjunto de dados deve conter informações sobre diversos assuntos.

---

## 🌐 Diversidade

São utilizadas informações provenientes de várias fontes.

Exemplos:

- Livros
- Sites
- Artigos
- Documentação
- Conteúdo público

---

## 🧠 Generalização

O objetivo é criar um modelo capaz de resolver diferentes tipos de tarefas, mesmo sem treinamento específico.

---

## 🧹 Preparação dos dados

Antes do treinamento, normalmente é realizada:

- Limpeza
- Padronização
- Remoção de inconsistências
- Anonimização de dados sensíveis

---

# 🎯 Preparação de dados para ajuste fino

No ajuste fino, a preparação dos dados é muito mais direcionada.

O foco deixa de ser quantidade e passa a ser qualidade.

---

## 🎯 Especificidade

Os dados devem estar diretamente relacionados ao problema que será resolvido.

Exemplos:

- Histórico de atendimento
- Contratos jurídicos
- Prontuários médicos
- Dados de vendas

---

## ⭐ Alta relevância

Cada exemplo utilizado deve contribuir para melhorar exatamente a tarefa desejada.

Dados irrelevantes reduzem a eficiência do ajuste fino.

---

## 💎 Qualidade acima da quantidade

Diferentemente do pré-treinamento, um conjunto menor de dados pode produzir excelentes resultados, desde que seja cuidadosamente selecionado.

---

# 🛠️ Principais etapas da preparação dos dados

## 📂 Curadoria dos dados

Selecionar apenas dados realmente úteis para o problema.

---

## 🏷️ Rotulagem

Adicionar rótulos corretos aos exemplos utilizados.

A qualidade da rotulagem influencia diretamente o desempenho do modelo.

---

## 🛡️ Governança e conformidade

Garantir que os dados estejam de acordo com:

- Regulamentações
- Privacidade
- Políticas internas
- LGPD e demais legislações aplicáveis

---

## ⚖️ Representatividade e mitigação de vieses

Verificar se os dados representam adequadamente diferentes grupos e cenários.

Isso reduz a possibilidade de introduzir novos vieses durante o ajuste fino.

---

## 🔄 Integração de feedback

Quando utilizado **RLHF**, o feedback humano passa a fazer parte do treinamento.

Esse feedback permite melhorar continuamente a qualidade das respostas.

---

## 🔁 Comparações importantes

---

### Pré-treinamento vs Ajuste fino

| Pré-treinamento | Ajuste fino |
|-----------------|-------------|
| Conhecimento geral | Conhecimento específico |
| Grandes volumes de dados | Pequenos conjuntos especializados |
| Diversos domínios | Um domínio específico |
| Alto custo computacional | Custo bem menor |

---

### Ajuste de instruções vs RLHF

| Ajuste de instruções | RLHF |
|----------------------|-------|
| Usa exemplos de prompts e respostas | Usa avaliações humanas |
| Ensina a seguir instruções | Ensina preferências humanas |
| Mais simples | Mais complexo |
| Muito usado em chatbots | Muito usado para alinhamento do modelo |

---

### Ajuste fino vs Pré-treinamento contínuo

| Ajuste fino | Pré-treinamento contínuo |
|--------------|--------------------------|
| Especializa o modelo | Atualiza o conhecimento geral |
| Focado em uma tarefa | Focado em novos dados |
| Usa dados específicos do domínio | Usa novos dados em larga escala |

---

## 🧠 Conceitos importantes para prova

- Fine-tuning adapta um modelo pré-treinado para uma tarefa específica.
- O objetivo é especializar, e não criar um modelo do zero.
- Instruction Tuning utiliza pares de instrução e resposta.
- RLHF utiliza feedback humano para alinhar o comportamento do modelo.
- Transfer Learning reutiliza conhecimento previamente adquirido.
- No ajuste fino, qualidade dos dados é mais importante que quantidade.
- Curadoria, rotulagem e mitigação de vieses são etapas fundamentais.

---

## ⚠️ Pegadinhas comuns

- Fine-tuning **não significa** treinar um modelo do zero.
- RLHF é uma forma de ajuste fino baseada em feedback humano.
- Pré-treinamento contínuo não substitui o ajuste fino.
- Mais dados não significam necessariamente melhores resultados.
- Dados mal rotulados podem piorar o desempenho do modelo.

---

## 🔁 Resumo rápido

- Fine-tuning adapta um modelo para um domínio específico.
- Existem diferentes técnicas, como Instruction Tuning, RLHF, Transfer Learning e Pré-treinamento Contínuo.
- O foco do ajuste fino é especialização.
- A qualidade dos dados é mais importante que sua quantidade.
- Curadoria, rotulagem e governança são essenciais para um bom ajuste fino.

---

## 📌 Status de aprendizado

- [ ] Entendo o que é Fine-tuning
- [ ] Sei por que utilizar ajuste fino
- [ ] Conheço as principais abordagens de ajuste fino
- [ ] Entendo a diferença entre pré-treinamento e ajuste fino
- [ ] Sei quais etapas são importantes na preparação dos dados
```
