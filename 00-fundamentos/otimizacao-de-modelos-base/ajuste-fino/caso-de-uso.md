# 👔 Caso de Negócio — Otimização de Modelo de Base com Ajuste Fino

A **AnyCompany** é uma varejista de moda on-line que deseja melhorar a experiência de compra de seus clientes utilizando **IA generativa**.

Apesar de possuir um grande catálogo de produtos, a empresa enfrenta dificuldades para oferecer recomendações realmente personalizadas.

Como consequência, observa:

- 🛒 Alto índice de abandono de carrinhos
- 🔄 Baixa taxa de recompra
- 😕 Dificuldade dos clientes em encontrar produtos adequados ao seu estilo
- 📉 Baixo engajamento durante a navegação

Para resolver esse problema, a empresa decide utilizar um **LLM ajustado com dados próprios**, permitindo recomendações e conteúdos mais personalizados.

---

# 🎯 Objetivos do negócio

A AnyCompany pretende utilizar IA generativa para tornar a experiência de compra mais personalizada e aumentar seus resultados comerciais.

Os principais objetivos são:

- Melhorar o engajamento dos clientes
- Reduzir o abandono de carrinhos
- Aumentar as compras recorrentes
- Oferecer recomendações mais relevantes
- Personalizar descrições e interações

---

# 📊 KPIs monitorados

Para medir o sucesso da solução, a empresa acompanha três indicadores principais.

## 💰 Taxa de conversão

Mede o percentual de visitantes que efetivamente realizam uma compra.

Objetivo:

- Aumentar o número de compras por visita ao site.

---

## 🛍️ Valor médio do pedido (Average Order Value)

Mede o valor médio gasto em cada compra.

Objetivo:

- Incentivar compras maiores.
- Aumentar o ticket médio das vendas.

---

## 🔄 Taxa de retenção de clientes

Mede a porcentagem de clientes que voltam a comprar.

Objetivo:

- Aumentar a fidelização.
- Estimular compras recorrentes.

---

# 💡 A solução

Para atingir esses objetivos, a AnyCompany utiliza um **Grande Modelo de Linguagem (LLM)** especializado no domínio da moda.

O modelo será responsável por diversas tarefas durante a experiência de compra.

## ✨ Geração dinâmica de descrições

As descrições dos produtos deixam de ser estáticas.

O modelo gera descrições personalizadas considerando:

- Preferências do cliente
- Histórico de compras
- Estilo pessoal
- Comportamento de navegação

---

## 🎯 Recomendações personalizadas

O LLM trabalha em conjunto com o mecanismo de recomendação da loja.

Assim, cada cliente visualiza produtos mais alinhados ao seu perfil.

Exemplos:

- Produtos semelhantes aos já comprados
- Itens complementares
- Promoções relevantes
- Novidades compatíveis com o estilo do cliente

---

## 💬 Interações inteligentes

O modelo também melhora o atendimento automatizado.

Pode oferecer:

- Sugestões de produtos
- Dicas de combinações
- Recomendações personalizadas
- Respostas em linguagem natural

---

# 📚 Uso de dados específicos

Diferentemente de um modelo genérico, a AnyCompany realiza **ajuste fino (Fine-tuning)** utilizando dados da própria empresa.

Entre eles:

- Histórico de compras
- Dados transacionais
- Feedback dos clientes
- Curtidas
- Cliques
- Produtos visualizados
- Compras anteriores

Esses dados permitem que o modelo aprenda características específicas do negócio e ofereça respostas muito mais relevantes.

---

# 🔄 Aprendizado contínuo

O comportamento dos consumidores muda constantemente.

Por isso, a empresa realiza ajustes periódicos do modelo utilizando novos dados.

Esse processo permite acompanhar:

- Novas tendências da moda
- Mudanças de comportamento dos clientes
- Novos produtos
- Novas preferências de compra

Com isso, o sistema mantém recomendações atualizadas sem precisar reconstruir o modelo do zero.

---

# ⚙️ Funcionamento da solução

A arquitetura pode ser dividida em três etapas principais.

<img width="1126" height="651" alt="image" src="https://github.com/user-attachments/assets/d2b6e506-c716-407c-85c3-82a5386964c7" />

---

## 1️⃣ Ingestão de dados

Nesta etapa são coletadas informações sobre o comportamento dos clientes.

Entre elas:

- Cliques
- Compras
- Produtos visualizados
- Comentários
- Avaliações
- Feedback dos usuários

Esses dados ajudam a identificar padrões e preferências individuais.

---

## 2️⃣ Saídas do modelo

Com base nas informações coletadas, o modelo gera conteúdo personalizado.

Exemplos:

- Descrições dinâmicas de produtos
- Recomendações individuais
- Exibição personalizada do catálogo
- Promoções específicas para cada cliente

Cada usuário passa a visualizar uma experiência diferente dentro da loja.

---

## 3️⃣ Circuito de feedback

Após cada interação, novos dados retornam ao sistema.

Essas informações são utilizadas para melhorar continuamente o modelo.

Exemplos:

- Produtos comprados
- Produtos ignorados
- Tempo de navegação
- Avaliações dos clientes
- Novos comentários

Esse ciclo mantém o modelo atualizado e cada vez mais preciso.

---

# 🎯 Por que utilizar ajuste fino?

Embora um LLM genérico compreenda linguagem natural, ele não conhece as particularidades da AnyCompany.

O ajuste fino permite ensinar ao modelo:

- Linguagem utilizada pela empresa
- Estilo das descrições
- Preferências dos clientes
- Características dos produtos
- Contexto específico do negócio

O resultado é uma IA muito mais especializada do que um modelo genérico.

---

## 🔁 Comparações importantes

---

### Modelo genérico vs Modelo ajustado

| Modelo genérico | Modelo ajustado |
|-----------------|-----------------|
| Conhecimento geral | Conhecimento específico do negócio |
| Respostas genéricas | Respostas personalizadas |
| Não conhece clientes | Aprende com dados da empresa |
| Pouca personalização | Alta personalização |

---

### RAG vs Ajuste fino

| RAG | Ajuste fino |
|------|-------------|
| Recupera informações externas | Ensina novos comportamentos ao modelo |
| Usa base de conhecimento | Usa dados para treinar o modelo |
| Não altera os pesos do modelo | Altera os pesos durante o treinamento |
| Ideal para informações atualizadas | Ideal para especialização em um domínio |

---

## 🧠 Conceitos importantes para prova

- O ajuste fino utiliza dados específicos da empresa para especializar o modelo.
- A AnyCompany utiliza dados de compras, cliques e feedback dos clientes.
- O objetivo é aumentar personalização e melhorar indicadores de negócio.
- O modelo gera descrições dinâmicas e recomendações personalizadas.
- O circuito de feedback permite melhorar continuamente o desempenho do modelo.

---

## ⚠️ Pegadinhas comuns

- Ajuste fino **não significa** treinar um modelo do zero.
- O modelo continua sendo um LLM pré-treinado.
- Nem toda personalização exige ajuste fino; em muitos casos, RAG é suficiente.
- O feedback dos usuários pode ser utilizado para novos ciclos de ajuste fino.
- Ajuste fino melhora o conhecimento específico do domínio, não apenas a recuperação de informações.

---

## 🔁 Resumo rápido

- A AnyCompany usa ajuste fino para personalizar a experiência de compra.
- O modelo aprende com dados reais da empresa.
- Gera descrições e recomendações personalizadas.
- O sistema utiliza ingestão de dados, geração de respostas e circuito de feedback.
- O objetivo é aumentar conversão, ticket médio e retenção de clientes.

---

## 📌 Status de aprendizado

- [ ] Entendo o caso de negócio da AnyCompany
- [ ] Sei por que foi escolhido ajuste fino
- [ ] Entendo quais dados são utilizados no treinamento
- [ ] Sei como funciona o circuito de feedback
- [ ] Consigo explicar por que o ajuste fino melhora a personalização
