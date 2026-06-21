# 🔄 Ciclo de Vida de Desenvolvimento de Machine Learning

<img width="1022" height="496" alt="image" src="https://github.com/user-attachments/assets/b109ab9b-00a7-4aad-9af1-e722b8263d96" />


O **ciclo de vida de Machine Learning (ML Lifecycle)** representa todo o processo necessário para desenvolver, implantar, monitorar e manter um modelo de Machine Learning em produção.
É um processo **iterativo**, pois frequentemente é necessário voltar às etapas anteriores para melhorar o desempenho do modelo.

---

# 🗺️ Etapas do ciclo de vida de ML

O ciclo de vida de ML normalmente é composto pelas seguintes etapas:

1. 🎯 Definição das metas de negócio
2. 🧩 Formulação do problema de ML
3. 📊 Processamento dos dados
4. 🤖 Desenvolvimento do modelo
5. 🚀 Implantação do modelo
6. 📈 Monitoramento
7. 🔄 Retreinamento

---

# 🎯 1. Definição das Metas de Negócio

Todo projeto de Machine Learning começa com um problema de negócio, e não com tecnologia.

Nesta etapa são definidos:

- Objetivos do projeto
- Valor esperado para a empresa
- Orçamento
- Critérios de sucesso
- KPIs (Key Performance Indicators)

Os KPIs permitem medir se o modelo realmente resolveu o problema proposto.

---

# 🧩 2. Formulação do Problema de Machine Learning

Após entender o problema de negócio, ele precisa ser convertido em um problema de Machine Learning.

Essa etapa envolve responder perguntas como:

- ML realmente é a solução?
- Existem dados suficientes?
- Há conhecimento técnico disponível?
- O problema é de classificação, regressão ou outro tipo?

Normalmente participam dessa fase:

- Cientistas de Dados
- Engenheiros de Dados
- Arquitetos de ML
- Especialistas do negócio (SMEs)

---

# 📊 3. Processamento dos Dados

Depois que o problema está definido, inicia-se a preparação dos dados.

O objetivo é transformar dados brutos em informações utilizáveis pelo modelo.

As principais atividades são:

- Coleta de dados
- Integração de dados
- Pré-processamento
- Visualização
- Engenharia de atributos (Feature Engineering)

---

## 📥 Coleta e integração de dados

Consiste em reunir dados de diferentes fontes e centralizá-los.

Objetivos:

- Garantir disponibilidade
- Unificar informações
- Eliminar inconsistências

---

## 🧹 Pré-processamento

É a etapa de limpeza e preparação dos dados.

Inclui atividades como:

- Remover dados inválidos
- Corrigir valores ausentes
- Normalizar dados
- Padronizar formatos

Um bom pré-processamento melhora significativamente a qualidade do modelo.

---

## 📈 Visualização de dados

Consiste em explorar os dados visualmente para compreender seus padrões.

Exemplos:

- Distribuição das classes
- Frequência de categorias
- Correlações
- Outliers

Essa análise ajuda a identificar problemas antes do treinamento.

---

## 🏗️ Engenharia de atributos (Feature Engineering)

É o processo de criar, transformar ou selecionar atributos que serão utilizados pelo modelo.

Exemplos:

- Criar novas variáveis
- Combinar atributos
- Remover atributos irrelevantes
- Selecionar apenas informações importantes

Uma boa engenharia de atributos costuma gerar ganhos maiores do que simplesmente trocar de algoritmo.

---

# 🤖 4. Desenvolvimento do Modelo

Após preparar os dados, inicia-se o treinamento do modelo.

Essa fase é composta por:

- Treinamento
- Avaliação
- Ajuste
- Novo treinamento (quando necessário)

É uma etapa altamente iterativa.

---

## 🏋️ Treinamento

O algoritmo aprende padrões presentes nos dados.

Quanto melhores forem os dados e os atributos, melhores tendem a ser os resultados.

---

## 📊 Divisão dos dados

Antes do treinamento, os dados normalmente são divididos em:

- Treinamento → 80%
- Validação → 10%
- Teste → 10%

Outra divisão bastante comum é:

- 70%
- 15%
- 15%

Essa separação evita que o modelo apenas memorize os dados.

---

## 🧪 Avaliação

Após o treinamento, o modelo é testado utilizando dados que ele nunca viu.

O objetivo é verificar sua capacidade de generalização.

Avaliar usando os mesmos dados do treinamento produz resultados enganosos.

---

## ⚙️ Ajuste do modelo

Caso o desempenho não seja satisfatório, inicia-se uma fase de otimização.

Pode incluir:

- Ajuste de hiperparâmetros
- Novas features
- Remoção de atributos
- Novos dados

Depois disso, o modelo é treinado novamente.

---

# 🔄 Retreinamento

Nem sempre o modelo atinge as metas de negócio na primeira tentativa.

Quando isso acontece, pode ser necessário:

- Revisar os dados
- Melhorar os atributos
- Ajustar hiperparâmetros
- Coletar novos dados

Esse ciclo pode ocorrer diversas vezes.

---

# 🚀 5. Implantação (Deployment)

Quando o desempenho é considerado satisfatório, o modelo é colocado em produção.

A partir desse momento ele passa a:

- Fazer inferências
- Realizar previsões
- Apoiar decisões do negócio

---

# 📈 6. Monitoramento

Após a implantação, o trabalho não termina.

É necessário acompanhar continuamente:

- Precisão
- Performance
- Drift dos dados
- Drift do modelo
- Erros
- Disponibilidade

Caso seja detectada degradação no desempenho, inicia-se um novo ciclo.

---

# 🔄 7. Retreinamento Contínuo

Com o passar do tempo:

- Os dados mudam
- O comportamento dos usuários muda
- O ambiente muda

Por isso, muitos modelos precisam ser retreinados periodicamente.

Esse processo garante que o modelo continue produzindo boas previsões.

---

# 🏢 Caso de Uso: Call Center da Amazon

A Amazon utilizou Machine Learning para melhorar o roteamento das ligações de atendimento ao cliente.

Antes da IA, o cliente navegava por longos menus telefônicos ("Pressione 1...", "Pressione 2..."), o que frequentemente resultava em encaminhamento para o atendente errado.

O objetivo era reduzir transferências de chamadas e melhorar a experiência do cliente.

---

## 🎯 Meta de negócio
<img width="707" height="256" alt="image" src="https://github.com/user-attachments/assets/ab00540d-c7f4-48e2-b80d-768e2bbf25df" />

Problema:

- Muitas transferências
- Alto custo operacional
- Atendimento lento
- Experiência ruim para o cliente

Objetivo:

Encaminhar o cliente diretamente ao atendente mais adequado.

---

## 🧩 Formulação do problema

Problema de negócio:

"Como encaminhar corretamente cada cliente?"

Problema de ML:

Prever qual habilidade do atendente melhor resolverá aquela chamada.

Trata-se de um problema de **classificação multiclasse**, pois existem diversas categorias possíveis de atendimento.

---

## 📥 Coleta de dados

Foram utilizados dados históricos das ligações.

Exemplos de atributos:

- Último pedido do cliente
- Cliente possui Kindle?
- Cliente é Prime?
- Histórico de compras
- Histórico de atendimento

Como existiam rótulos conhecidos (tipo correto de atendimento), utilizou-se **Aprendizado Supervisionado**.

---

## 🧹 Pré-processamento

Foram realizadas atividades como:

- Limpeza dos dados
- Remoção de inconsistências
- Agrupamento de categorias semelhantes

<img width="714" height="227" alt="image" src="https://github.com/user-attachments/assets/193b52ef-6949-492b-9e0c-64f74d50ee6e" />

Exemplo:

Diversos tipos de suporte ao Kindle foram agrupados em uma única categoria.

Isso simplificou o treinamento.

---

## 📊 Visualização

A equipe analisou estatísticas como:

- Percentual de chamadas sobre devoluções
- Chamadas relacionadas ao Prime
- Chamadas sobre Kindle

Essa etapa ajudou a compreender melhor o conjunto de dados.

---

## 🤖 Treinamento

Os dados foram divididos entre:

- Treinamento
- Validação
- Teste

O modelo foi treinado para prever corretamente qual atendente deveria receber cada ligação.

---

## ⚙️ Ajuste

Após cada treinamento foram realizados:

- Ajuste de hiperparâmetros
- Engenharia de atributos
- Novo treinamento

Esse ciclo foi repetido até atingir os resultados desejados.

---

## 🚀 Implantação

Após apresentar bom desempenho nos testes, o modelo foi colocado em produção.

Resultado:

Os clientes passaram a ser encaminhados corretamente já na primeira tentativa.

Isso reduziu:

- Transferências
- Tempo de atendimento
- Custos operacionais

Além de melhorar significativamente a experiência dos clientes.

---

## 🔁 Comparações importantes

---

### Problema de negócio vs Problema de Machine Learning

| Problema de negócio | Problema de ML |
|----------------------|----------------|
| Define o objetivo da empresa | Define como a IA resolverá o problema |
| Focado em valor para o negócio | Focado em previsão ou aprendizado |
| Ex.: reduzir transferências | Ex.: prever o atendente correto |

---

### Treinamento vs Avaliação

| Treinamento | Avaliação |
|-------------|-----------|
| Modelo aprende padrões | Modelo é testado |
| Usa dados de treinamento | Usa dados nunca vistos |
| Ajusta pesos internos | Mede capacidade de generalização |

---

### Implantação vs Monitoramento

| Implantação | Monitoramento |
|-------------|---------------|
| Modelo entra em produção | Modelo é acompanhado continuamente |
| Faz previsões reais | Detecta perda de desempenho |
| Início da operação | Garante qualidade ao longo do tempo |

---

## 🧠 Conceitos importantes para prova

- Todo projeto de ML começa com um **problema de negócio**
- O problema de negócio deve ser convertido em um **problema de Machine Learning**
- O processamento dos dados inclui:
  - Coleta
  - Pré-processamento
  - Visualização
  - Engenharia de atributos
- Nunca avalie um modelo utilizando os mesmos dados usados no treinamento
- A divisão mais comum dos dados é **80/10/10** ou **70/15/15**
- O desenvolvimento do modelo é um processo **iterativo**
- Após a implantação, o modelo deve ser monitorado continuamente
- Mudanças nos dados podem exigir **retreinamento**

---

## ⚠️ Pegadinhas comuns

- Machine Learning **não começa pelo treinamento**, mas pelas metas de negócio
- Implantar o modelo **não encerra** o ciclo de vida
- Avaliar usando os dados de treinamento gera resultados enganosos
- Engenharia de atributos pode melhorar mais o modelo do que trocar de algoritmo
- Retreinamento faz parte do ciclo normal de ML
- O caso do Call Center da Amazon é um problema de **classificação multiclasse**, não regressão

---

## 🔁 Resumo rápido

- O ciclo de vida de ML possui sete etapas principais
- Tudo começa com um problema de negócio
- Os dados precisam ser preparados antes do treinamento
- O modelo passa por treinamento, avaliação e ajustes iterativos
- Após atingir bom desempenho, é implantado em produção
- O monitoramento garante que o modelo continue funcionando corretamente
- Quando necessário, o modelo é retreinado para manter sua qualidade

---

## 📌 Status de aprendizado

- [ ] Entendo as etapas do ciclo de vida de ML
- [ ] Sei diferenciar problema de negócio e problema de ML
- [ ] Entendo o processamento dos dados
- [ ] Sei como ocorre o desenvolvimento do modelo
- [ ] Entendo a importância da avaliação e do monitoramento
- [ ] Sei quando o retreinamento é necessário
- [ ] Compreendo o caso de uso do Call Center da Amazon

```
