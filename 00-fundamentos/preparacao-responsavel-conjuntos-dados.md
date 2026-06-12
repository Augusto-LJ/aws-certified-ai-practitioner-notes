# 🗂️ Preparação responsável de conjuntos de dados

A preparação responsável dos dados é um dos pilares da IA Responsável (Responsible AI). Modelos de IA dependem diretamente da qualidade dos dados utilizados durante o treinamento, portanto conjuntos de dados mal preparados podem gerar sistemas enviesados, injustos ou imprecisos.

## 🎯 Objetivo

Garantir que os conjuntos de dados utilizados no treinamento sejam:

- Balanceados
- Representativos
- Inclusivos
- Diversos
- Livres de vieses desnecessários
- Adequados ao caso de uso

## ⚖️ Balanceamento de conjuntos de dados

Um conjunto de dados balanceado (Balanced Dataset) representa adequadamente todos os grupos, categorias ou características relevantes para o problema.

Quando um grupo está sub-representado, o modelo tende a apresentar menor desempenho para esse grupo.

### Exemplo

Um modelo treinado principalmente com dados de pessoas de meia idade pode apresentar menor precisão ao realizar previsões para:

- Crianças
- Jovens
- Idosos

Isso ocorre porque esses grupos não foram suficientemente representados durante o treinamento.

### Benefícios do balanceamento

- Redução de vieses (Bias)
- Maior imparcialidade (Fairness)
- Melhor generalização do modelo
- Resultados mais confiáveis
- Menor risco de discriminação

### Casos de uso sensíveis

O balanceamento é especialmente importante em aplicações como:

- Contratação de funcionários
- Aprovação de crédito e empréstimos
- Saúde
- Justiça criminal
- Educação

Nesses cenários, decisões enviesadas podem gerar impactos sociais e legais significativos.

## 🌎 Coleta de dados inclusivos e diversos

A inclusão e diversidade (Inclusion and Diversity) durante a coleta de dados ajudam a garantir que o modelo represente corretamente a realidade.

Os dados devem incluir:

- Diferentes grupos demográficos
- Diferentes perspectivas
- Diferentes regiões geográficas
- Diferentes contextos sociais
- Diferentes fontes de informação

### Exemplo

Ao criar um modelo para análise de pessoas, o conjunto de dados deve incluir adequadamente:

- Diferentes faixas etárias
- Diferentes gêneros
- Diferentes grupos populacionais
- Diferentes contextos culturais

Caso contrário, o modelo poderá favorecer grupos mais representados.

### Importância

A coleta inclusiva ajuda a promover:

- Imparcialidade (Fairness)
- Transparência (Transparency)
- Responsabilidade (Accountability)
- Confiabilidade (Trustworthiness)

## 🏷️ Curadoria de dados
<img width="919" height="96" alt="image" src="https://github.com/user-attachments/assets/40cf4b27-fd61-4cae-98eb-fdd73949fa61" />


A curadoria de dados (Data Curation) é o processo de preparar os dados para uso no treinamento dos modelos.

Ela envolve:

- Organização
- Rotulagem (Labeling)
- Limpeza
- Transformação
- Validação

O objetivo é garantir que os dados sejam:

- Relevantes
- Precisos
- Consistentes
- Representativos

## 🔧 Pré-processamento de dados

O pré-processamento (Data Preprocessing) prepara os dados antes do treinamento.

Principais atividades:

- Limpeza de dados (Data Cleaning)
- Correção de inconsistências
- Remoção de registros inválidos
- Normalização (Normalization)
- Seleção de atributos (Feature Selection)

### Benefícios

- Reduz ruídos nos dados
- Melhora a qualidade do treinamento
- Ajuda a reduzir vieses

## 📈 Aumento de dados

O aumento de dados (Data Augmentation) consiste em criar novas amostras para complementar grupos sub-representados.

### Objetivos

- Melhorar o balanceamento
- Aumentar a diversidade
- Reduzir vieses

### Exemplo

Se houver poucas imagens de uma determinada categoria, novas imagens podem ser geradas através de:

- Rotação
- Espelhamento
- Recorte
- Alterações de iluminação

## 🔍 Auditoria regular

Os conjuntos de dados devem ser auditados periodicamente.

### O que verificar

- Presença de vieses
- Mudanças na distribuição dos dados
- Qualidade dos rótulos
- Representatividade dos grupos

### Benefícios

- Mantém a qualidade dos dados
- Identifica problemas precocemente
- Permite ações corretivas antes do treinamento

## 🎯 Balanceamento baseado no caso de uso

Nem sempre "balanceado" significa distribuir igualmente todos os grupos.

O balanceamento deve refletir o objetivo do sistema.

### Exemplo

Se o objetivo for desenvolver um sistema para:

- Diagnóstico de câncer infantil

O conjunto de dados deve ser composto principalmente por:

- Crianças

Nesse caso, incluir grande quantidade de dados de adultos não contribuiria para o objetivo do modelo.

### Regra importante para a prova

Os dados devem ser balanceados de acordo com o caso de uso pretendido (Intended Use Case).

## 🛠️ Ferramentas AWS

### Amazon SageMaker Clarify

Utilizado para:

- Detectar vieses nos dados
- Detectar vieses nos modelos
- Avaliar métricas de imparcialidade
- Gerar relatórios de explicabilidade

### Amazon SageMaker Data Wrangler

Utilizado para:

- Coleta e preparação de dados
- Transformação de dados
- Limpeza de dados
- Análise de qualidade dos dados
- Balanceamento de conjuntos de dados

## 📝 Resumo para a prova

- IA responsável exige conjuntos de dados balanceados.
- Dados devem ser inclusivos e diversos.
- Conjuntos de dados desbalanceados podem gerar vieses.
- A curadoria de dados envolve rotulagem, organização e pré-processamento.
- Pré-processamento ajuda a remover inconsistências e reduzir vieses.
- Data Augmentation pode ajudar grupos sub-representados.
- Auditorias periódicas ajudam a manter a qualidade dos dados.
- O balanceamento deve considerar o caso de uso pretendido.
- SageMaker Clarify auxilia na detecção de vieses.
- SageMaker Data Wrangler auxilia na preparação e transformação dos dados.
