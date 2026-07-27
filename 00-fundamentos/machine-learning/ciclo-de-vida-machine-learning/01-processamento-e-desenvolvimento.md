# 🛠️ Processamento e Desenvolvimento do Modelo

Após definir o problema de Machine Learning, inicia-se a preparação dos dados e o desenvolvimento do modelo.

Essas etapas são responsáveis por transformar dados brutos em um modelo capaz de realizar previsões com boa capacidade de generalização.

---

## 📊 Processamento dos dados

O objetivo do processamento dos dados é transformar dados brutos em informações utilizáveis pelo modelo.

As principais atividades são:

- Coleta de dados
- Integração de dados
- Pré-processamento
- Visualização
- Engenharia de atributos (Feature Engineering)

📌 A qualidade dessa etapa influencia diretamente o desempenho do modelo.

---

## 📥 Coleta e integração de dados

Consiste em reunir dados provenientes de diferentes fontes e centralizá-los.

### Objetivos

- Garantir disponibilidade dos dados
- Unificar informações
- Eliminar inconsistências

Uma boa coleta de dados aumenta as chances de o modelo aprender padrões representativos do problema.

---

## 🧹 Pré-processamento

É a etapa de limpeza e preparação dos dados antes do treinamento.

Inclui atividades como:

- Remover dados inválidos
- Corrigir valores ausentes
- Normalizar dados
- Padronizar formatos

📌 Um bom pré-processamento melhora significativamente a qualidade do modelo.

---

## 📈 Visualização de dados

Consiste em explorar os dados visualmente para compreender seus padrões antes do treinamento.

Exemplos de análises:

- Distribuição das classes
- Frequência de categorias
- Correlações
- Outliers

Essa análise ajuda a identificar problemas que podem comprometer o desempenho do modelo.

---

## 🏗️ Engenharia de atributos (Feature Engineering)

É o processo de criar, transformar ou selecionar atributos (features) que serão utilizados pelo modelo.

Exemplos:

- Criar novas variáveis
- Combinar atributos existentes
- Remover atributos irrelevantes
- Selecionar apenas informações importantes

📌 Uma boa engenharia de atributos costuma gerar ganhos maiores do que simplesmente trocar de algoritmo.

---

# 🤖 Desenvolvimento do modelo

Após preparar os dados, inicia-se o treinamento do modelo.

Essa fase é composta por:

- Treinamento
- Avaliação
- Ajuste
- Novo treinamento (quando necessário)

📌 É uma etapa altamente iterativa.

---

## 🏋️ Treinamento

Durante o treinamento, o algoritmo aprende padrões presentes nos dados.

Quanto melhores forem os dados e os atributos utilizados, melhores tendem a ser os resultados.

O objetivo é construir um modelo capaz de fazer boas previsões para dados que ele nunca viu anteriormente.

---

## 📊 Divisão dos dados

Antes do treinamento, os dados normalmente são divididos em três conjuntos:

- **Treinamento:** 80%
- **Validação:** 10%
- **Teste:** 10%

Outra divisão bastante comum é:

- **Treinamento:** 70%
- **Validação:** 15%
- **Teste:** 15%

Cada conjunto possui uma finalidade diferente:

- **Treinamento:** utilizado para ensinar o modelo.
- **Validação:** utilizado para ajustar o modelo durante o desenvolvimento.
- **Teste:** utilizado para medir o desempenho final em dados inéditos.

📌 Essa separação evita que o modelo apenas memorize os dados.

---

## 🧪 Avaliação

Após o treinamento, o modelo é avaliado utilizando dados que ele nunca viu.

O objetivo é verificar sua capacidade de generalização.

Avaliar utilizando os mesmos dados do treinamento produz resultados enganosos, pois o modelo pode apenas ter memorizado os exemplos.

---

## ⚙️ Ajuste do modelo

Caso o desempenho não seja satisfatório, inicia-se uma fase de otimização.

Pode incluir:

- Ajuste de hiperparâmetros
- Criação de novas features
- Remoção de atributos
- Coleta de novos dados

Após esses ajustes, o modelo é treinado novamente.

📌 É comum repetir esse processo diversas vezes até atingir os resultados esperados.

---

## 🚀 Implantação (Deployment)

Quando o desempenho é considerado satisfatório, o modelo é colocado em produção.

A partir desse momento ele passa a:

- Fazer inferências
- Realizar previsões
- Apoiar decisões do negócio

📌 A implantação não representa o fim do ciclo de vida do modelo.

---

## 📈 Monitoramento

Após a implantação, é necessário acompanhar continuamente o desempenho do modelo.

Os principais aspectos monitorados são:

- Precisão
- Performance
- Drift dos dados (Data Drift)
- Drift do modelo (Model Drift)
- Erros
- Disponibilidade

Caso seja detectada degradação no desempenho, inicia-se um novo ciclo de melhorias.

---

## 🔄 Retreinamento

Com o passar do tempo:

- Os dados mudam
- O comportamento dos usuários muda
- O ambiente muda

Por isso, muitos modelos precisam ser retreinados periodicamente.

O retreinamento garante que o modelo continue produzindo previsões confiáveis.

---

## 🔁 Comparações importantes

### Treinamento vs Avaliação

| Treinamento | Avaliação |
|-------------|-----------|
| Modelo aprende padrões | Modelo é testado |
| Usa dados de treinamento | Usa dados nunca vistos |
| Ajusta parâmetros internos | Mede capacidade de generalização |

---

### Implantação vs Monitoramento

| Implantação | Monitoramento |
|-------------|---------------|
| Modelo entra em produção | Modelo é acompanhado continuamente |
| Faz previsões reais | Detecta perda de desempenho |
| Início da operação | Garante qualidade ao longo do tempo |

---

## 🧠 Conceitos importantes para prova

- O processamento dos dados inclui:
  - Coleta
  - Integração
  - Pré-processamento
  - Visualização
  - Engenharia de atributos
- A qualidade dos dados impacta diretamente o desempenho do modelo
- Os dados normalmente são divididos em treinamento, validação e teste
- Nunca avalie um modelo utilizando os mesmos dados usados no treinamento
- O desenvolvimento do modelo é um processo iterativo
- Após a implantação, o modelo deve ser monitorado continuamente
- Mudanças nos dados podem exigir retreinamento

---

## ⚠️ Pegadinhas comuns

- Pré-processamento não é apenas remover dados inválidos
- Engenharia de atributos pode melhorar mais o modelo do que trocar de algoritmo
- Avaliar usando os dados de treinamento gera resultados enganosos
- Implantar o modelo não encerra o ciclo de vida
- Retreinamento faz parte do ciclo normal de Machine Learning

---

## 🔁 Resumo rápido

- Os dados passam por coleta, preparação e engenharia de atributos antes do treinamento
- O desenvolvimento envolve treinamento, avaliação e ajustes iterativos
- Os dados normalmente são divididos em treinamento, validação e teste
- Após a implantação, o modelo deve ser monitorado continuamente
- O retreinamento mantém o modelo atualizado conforme os dados evoluem

---

## 📌 Status de aprendizado

- [ ] Entendo as etapas do processamento dos dados
- [ ] Sei o que é Feature Engineering
- [ ] Entendo como os dados são divididos para treinamento
- [ ] Sei a diferença entre treinamento e avaliação
- [ ] Entendo a importância do monitoramento e do retreinamento
