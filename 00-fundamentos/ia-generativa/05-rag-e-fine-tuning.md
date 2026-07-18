# 🔄 RAG e Fine-tuning

## 📌 O que são

Existem duas principais formas de adaptar um **Foundation Model (FM)** para atender às necessidades de uma organização:

- **RAG (Retrieval-Augmented Generation)** → fornece informações externas ao modelo no momento da geração da resposta.
- **Fine-tuning (Ajuste fino)** → modifica o comportamento do modelo treinando-o com dados específicos.

📌 Ambos melhoram as respostas do modelo, mas funcionam de maneiras completamente diferentes.

---

# 🔄 Retrieval-Augmented Generation (RAG)

## 📌 O que é

A **Geração Aumentada por Recuperação (Retrieval-Augmented Generation - RAG)** é uma técnica que melhora as respostas de um modelo recuperando informações relevantes de fontes externas e adicionando essas informações ao prompt antes da geração da resposta.

📌 O modelo **não aprende** essas informações.

📌 Ele apenas as utiliza como contexto durante a inferência.

---

## ⚙️ Como funciona

Fluxo simplificado:

```text
Pergunta do usuário
        │
        ▼
Busca em documentos / Base de conhecimento
        │
        ▼
Recupera informações relevantes
        │
        ▼
Essas informações são adicionadas ao prompt
        │
        ▼
Foundation Model gera a resposta
```

---

## 🧠 O que o RAG faz

- Consulta documentos da empresa
- Pesquisa bases de conhecimento
- Recupera informações atualizadas
- Usa esse conteúdo para responder melhor

---

## 📌 Vantagens

- Não altera o modelo
- Dados sempre atualizados
- Implementação mais rápida
- Menor custo
- Fácil manutenção

---

## ⚠️ Limitações

- Depende da qualidade da base de conhecimento
- Se os documentos estiverem incorretos, a resposta também poderá estar
- Requer um mecanismo eficiente de busca

---

## 💡 Casos de uso

- Chatbots corporativos
- Pesquisa empresarial
- FAQ inteligente
- Consulta a documentação
- Assistentes internos
- Bases de conhecimento

---

# 🔄 Fine-tuning

## 📌 O que é

O **Fine-tuning (Ajuste fino)** é um processo de treinamento supervisionado que adapta um Foundation Model utilizando um conjunto menor de dados específicos.

O objetivo é especializar o modelo para determinado domínio ou comportamento.

📌 Diferente do RAG, o Fine-tuning **altera o modelo**.

---

## ⚙️ Como funciona

Fluxo simplificado:

```text
Foundation Model
        │
        ▼
Treinamento com dados específicos
        │
        ▼
Modelo especializado
```

---

## 🧠 O que muda

Durante o Fine-tuning:

- Os pesos do modelo são ajustados
- O modelo aprende novos padrões
- Passa a responder de forma mais consistente para aquele domínio

---

## 📌 Quando usar

Quando deseja que o modelo:

- Aprenda um estilo específico
- Utilize uma terminologia própria
- Responda seguindo um padrão
- Seja especializado em determinado domínio

---

## 💡 Exemplos

- Assistente jurídico
- Assistente médico
- Linguagem específica da empresa
- Padrão de escrita corporativo
- Geração de documentos padronizados

---

## 📌 Tipos de Fine-tuning

### Ajuste fino de instruções (Instruction Fine-tuning)

Treina o modelo utilizando exemplos de perguntas e respostas.

Objetivo:

- Melhorar a forma como o modelo segue instruções.

---

### RLHF (Reinforcement Learning from Human Feedback)

Aprendizado por reforço baseado em feedback humano.

O modelo aprende quais respostas são preferidas pelos usuários.

Objetivo:

- Tornar as respostas mais úteis
- Mais naturais
- Mais alinhadas às expectativas humanas

---

# 🔁 RAG vs Fine-tuning

## Diferenças principais

| RAG | Fine-tuning |
|------|-------------|
| Não altera o modelo | Altera o modelo |
| Usa dados externos | Aprende com novos dados |
| Dados podem ser atualizados facilmente | Requer novo treinamento para atualizar |
| Menor custo | Maior custo |
| Implementação rápida | Implementação mais demorada |
| Ideal para conhecimento atualizado | Ideal para mudar comportamento do modelo |

---

## Quando usar cada um

### Use RAG quando

- As informações mudam frequentemente
- Precisa acessar documentos internos
- Quer respostas baseadas em conhecimento atualizado
- Não deseja treinar um novo modelo

Exemplos:

- Políticas internas
- Manuais
- Wikis
- Base de conhecimento
- Documentação técnica

---

### Use Fine-tuning quando

- Deseja alterar o comportamento do modelo
- Precisa de respostas padronizadas
- Quer especializar o modelo em um domínio
- A informação não muda constantemente

Exemplos:

- Estilo de escrita
- Linguagem jurídica
- Linguagem médica
- Atendimento especializado

---

# 🧠 RAG no Amazon Bedrock

O Amazon Bedrock possui suporte nativo para RAG.

Normalmente o fluxo é:

```text
Usuário
      │
      ▼
Knowledge Base
      │
      ▼
Busca vetorial
      │
      ▼
Documentos relevantes
      │
      ▼
Foundation Model
      │
      ▼
Resposta
```

As **Knowledge Bases for Amazon Bedrock** simplificam a implementação de RAG, cuidando da indexação, recuperação dos documentos e integração com os modelos.

📌 O desenvolvedor não precisa implementar toda a infraestrutura manualmente.

---

# 🧠 Fine-tuning no Amazon Bedrock

O Amazon Bedrock também oferece suporte ao Fine-tuning para alguns Foundation Models.

Permite:

- Especializar modelos
- Melhorar respostas para um domínio específico
- Adaptar terminologia da empresa
- Ajustar o comportamento do modelo

📌 Nem todos os Foundation Models disponíveis no Bedrock suportam Fine-tuning.

---

# 🎯 Quando NÃO usar Fine-tuning

Evite Fine-tuning quando o problema é apenas fornecer informações atualizadas.

Exemplo:

❌ Manual da empresa muda toda semana.

Nesse caso, usar Fine-tuning exigiria treinar novamente o modelo frequentemente.

O ideal é utilizar **RAG**.

---

# 🎯 Quando NÃO usar RAG

Evite RAG quando deseja alterar permanentemente o comportamento do modelo.

Exemplo:

- Mudar o estilo de escrita
- Tornar o modelo especialista em um domínio específico
- Ensinar um formato fixo de resposta

Nesse caso, o ideal é utilizar **Fine-tuning**.

---

# 🧠 Conceitos importantes para prova

- RAG significa **Retrieval-Augmented Generation**.
- RAG busca informações externas durante a inferência.
- RAG **não altera** os pesos do modelo.
- Fine-tuning altera o modelo por meio de treinamento.
- RAG é mais barato e simples de manter.
- Fine-tuning é indicado para especializar o comportamento do modelo.
- No Amazon Bedrock há suporte tanto para **RAG** quanto para **Fine-tuning**.
- As **Knowledge Bases for Amazon Bedrock** facilitam a implementação de soluções com RAG.

---

# ⚠️ Pegadinhas comuns

- RAG **não treina** o modelo.
- Fine-tuning **não substitui** uma base de conhecimento.
- Fine-tuning não é necessário apenas para acessar documentos da empresa.
- RAG pode utilizar informações atualizadas sem novo treinamento.
- Fine-tuning geralmente possui custo e tempo de implementação maiores.

---

# 🔁 Resumo rápido

- **RAG**
  - Usa dados externos
  - Não altera o modelo
  - Ideal para informações atualizadas
  - Mais barato

- **Fine-tuning**
  - Treina o modelo
  - Altera seu comportamento
  - Ideal para especialização
  - Mais caro

---

# 📌 Status de aprendizado

- [ ] Sei explicar o que é RAG
- [ ] Sei explicar o que é Fine-tuning
- [ ] Entendo quando usar cada abordagem
- [ ] Sei a principal diferença entre RAG e Fine-tuning
- [ ] Entendo como o Amazon Bedrock suporta RAG e Fine-tuning
