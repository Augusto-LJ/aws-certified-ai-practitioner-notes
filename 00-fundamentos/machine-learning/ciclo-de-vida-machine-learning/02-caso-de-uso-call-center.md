# ☎️ Caso de Uso: Call Center da Amazon

## 📌 O contexto

A Amazon utilizou **Machine Learning (ML)** para melhorar o roteamento das ligações de atendimento ao cliente.

Antes da adoção de IA, o cliente precisava navegar por longos menus telefônicos ("Pressione 1...", "Pressione 2..."), o que frequentemente resultava no encaminhamento para o atendente errado.

O objetivo era utilizar ML para prever qual atendente teria maior probabilidade de resolver o problema logo na primeira tentativa.

---

## 🎯 Problema de negócio

<img width="707" height="256" alt="image" src="https://github.com/user-attachments/assets/ab00540d-c7f4-48e2-b80d-768e2bbf25df" />

Problemas identificados:

- Muitas transferências de chamadas
- Alto custo operacional
- Atendimento lento
- Experiência ruim para o cliente

Objetivo do negócio:

> Encaminhar cada cliente diretamente ao atendente mais adequado.

---

## 🧩 Formulação do problema de ML

Depois de definir o objetivo do negócio, ele foi convertido em um problema de Machine Learning.

### Problema de negócio

> Como encaminhar corretamente cada cliente?

### Problema de ML

> Prever qual habilidade do atendente melhor resolverá aquela chamada.

Trata-se de um problema de **classificação multiclasse (Multiclass Classification)**, pois existem diversas categorias possíveis de atendimento.

---

## 📥 Coleta de dados

Foram utilizados dados históricos das ligações realizadas pelos clientes.

Exemplos de atributos utilizados:

- Último pedido do cliente
- Cliente possui Kindle?
- Cliente é Amazon Prime?
- Histórico de compras
- Histórico de atendimento

Como existiam rótulos conhecidos (tipo correto de atendimento), utilizou-se **Aprendizado Supervisionado (Supervised Learning)**.

---

## 🧹 Pré-processamento

Foram realizadas diversas atividades para preparar os dados antes do treinamento:

- Limpeza dos dados
- Remoção de inconsistências
- Agrupamento de categorias semelhantes

<img width="714" height="227" alt="image" src="https://github.com/user-attachments/assets/193b52ef-6949-492b-9e0c-64f74d50ee6e" />

Exemplo:

Diversos tipos de suporte relacionados ao Kindle foram agrupados em uma única categoria.

Isso simplificou o treinamento e reduziu a complexidade do problema.

---

## 📊 Visualização dos dados

Antes do treinamento, a equipe analisou estatísticas importantes do conjunto de dados.

Exemplos:

- Percentual de chamadas sobre devoluções
- Chamadas relacionadas ao Amazon Prime
- Chamadas sobre Kindle

Essa etapa ajudou a compreender melhor os dados e identificar possíveis problemas antes do treinamento.

---

## 🤖 Treinamento

Os dados foram divididos em conjuntos de:

- Treinamento
- Validação
- Teste

O modelo foi treinado para prever corretamente qual atendente deveria receber cada ligação.

---

## ⚙️ Ajuste do modelo

Após cada treinamento foram realizados diversos ajustes, como:

- Ajuste de hiperparâmetros
- Engenharia de atributos (Feature Engineering)
- Novo treinamento

Esse processo foi repetido até que o desempenho atingisse os objetivos definidos pelo negócio.

---

## 🚀 Implantação

Após apresentar bom desempenho durante os testes, o modelo foi implantado em produção.

A partir desse momento, passou a realizar previsões em tempo real para direcionar as chamadas.

Resultados obtidos:

- Redução das transferências de chamadas
- Menor tempo de atendimento
- Redução dos custos operacionais
- Melhoria significativa da experiência dos clientes

---

## 🔁 Como esse exemplo percorre o ciclo de vida do ML

| Etapa | Aplicação no Call Center |
|--------|--------------------------|
| Meta de negócio | Reduzir transferências e melhorar o atendimento |
| Formulação do problema | Prever o atendente mais adequado |
| Processamento dos dados | Coleta, limpeza e preparação dos históricos |
| Desenvolvimento | Treinamento, avaliação e ajustes do modelo |
| Implantação | Modelo utilizado para rotear chamadas |
| Monitoramento | Acompanhamento contínuo do desempenho |
| Retreinamento | Atualização do modelo quando necessário |

---

## 🧠 Conceitos importantes para prova

- Todo projeto de ML começa com um **problema de negócio**
- O problema de negócio deve ser transformado em um **problema de Machine Learning**
- O caso do Call Center utiliza **Aprendizado Supervisionado**
- Trata-se de um problema de **Classificação Multiclasse**
- A preparação dos dados foi essencial antes do treinamento
- O desenvolvimento do modelo foi iterativo
- Após a implantação, o modelo continua sendo monitorado e pode ser retreinado

---

## ⚠️ Pegadinhas comuns

- O problema do Call Center **não é regressão**, e sim **classificação multiclasse**
- O treinamento não começou imediatamente; primeiro foi definido o problema de negócio
- A implantação **não encerra** o ciclo de vida do modelo
- O modelo continua sendo monitorado e atualizado após entrar em produção
- A qualidade dos dados foi determinante para o sucesso do projeto

---

## ✅ Resumo para prova

- Objetivo: encaminhar cada cliente ao atendente correto
- Problema de ML: prever a categoria de atendimento (**classificação multiclasse**)
- Utiliza **Aprendizado Supervisionado**
- Passa por todas as etapas do ciclo de vida:
  - Definição do problema
  - Coleta e preparação dos dados
  - Treinamento
  - Ajustes
  - Implantação
  - Monitoramento
  - Retreinamento
- Demonstra como o ML pode gerar ganhos operacionais e melhorar a experiência do cliente

---

## 📌 Status de aprendizado

- [ ] Entendo o problema de negócio do Call Center da Amazon
- [ ] Sei por que é um problema de classificação multiclasse
- [ ] Entendo como o caso percorre todas as etapas do ciclo de vida de ML
- [ ] Consigo relacionar cada etapa do ciclo de vida ao exemplo do Call Center
