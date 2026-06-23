# 🤖 Seleção de um Modelo de Base (Foundation Model - FM)

Após definir o caso de uso, a próxima etapa do ciclo de vida de uma aplicação de IA generativa é **selecionar um Modelo de Base (Foundation Model - FM)**.

<img width="911" height="106" alt="image" src="https://github.com/user-attachments/assets/1f8cb110-8468-44bd-91d5-0ba48991a1c4" />

Essa decisão é extremamente importante, pois influencia diretamente:

- 🎯 Qualidade das respostas
- ⚡ Desempenho
- 💰 Custos
- 📈 Escalabilidade
- 🛡️ Robustez
- 🔧 Facilidade de personalização

Nesta etapa, uma das primeiras decisões é escolher entre:

- Utilizar um **modelo pré-treinado**
- Desenvolver um **modelo do zero**

Na prática, a maioria das aplicações utiliza modelos pré-treinados devido ao menor custo e ao tempo reduzido de desenvolvimento.

---

# 🧠 Modelos Pré-treinados

Modelos pré-treinados já foram treinados utilizando enormes volumes de dados.

Isso permite que eles já possuam conhecimento geral sobre linguagem, imagens, código ou outros domínios.

Posteriormente, eles podem ser:

- Utilizados diretamente
- Ajustados (Fine-tuning)
- Personalizados para tarefas específicas

## ✅ Vantagens

- Menor tempo de desenvolvimento
- Menor custo de treinamento
- Excelente desempenho geral
- Grande quantidade de conhecimento prévio

## ⚠️ Desvantagens

- Podem conter vieses
- Nem sempre conhecem bem um domínio específico
- Algumas personalizações podem exigir custos adicionais

---

# 📋 Critérios para Seleção de um Modelo Pré-treinado

A escolha do modelo depende diretamente do caso de uso.

Diversos critérios devem ser analisados.

---

## 💰 Custo

É necessário avaliar o custo total de utilização.

Pode incluir:

- Licenciamento
- Inferência
- Ajuste fino (Fine-tuning)
- Recursos computacionais

Um modelo melhor nem sempre é o mais vantajoso financeiramente.

---

## 🎨 Modalidade

Refere-se ao tipo de conteúdo que o modelo consegue gerar.

Pode ser:

- 📝 Texto
- 🖼️ Imagem
- 🔊 Áudio
- 🎥 Multimodal (texto + imagem + áudio)

A modalidade deve ser compatível com a aplicação.

---

## ⚡ Latência

Latência é o tempo que o modelo leva para responder.

Algumas aplicações exigem respostas quase instantâneas.

Exemplos:

- Chatbots
- Assistentes virtuais
- Atendimento em tempo real

Outras aplicações podem tolerar tempos maiores.

---

## 🌎 Suporte a múltiplos idiomas

Caso a aplicação atenda usuários internacionais, o modelo deve oferecer suporte aos idiomas desejados.

Alguns modelos possuem excelente desempenho em inglês, mas desempenho inferior em outros idiomas.

---

## 📦 Tamanho do modelo

Modelos maiores normalmente apresentam:

- Melhor desempenho
- Maior capacidade de raciocínio

Entretanto também exigem:

- Mais memória
- Mais processamento
- Maior custo de inferência

É necessário equilibrar qualidade e custo.

---

## 🧩 Complexidade do modelo

Modelos muito sofisticados conseguem resolver tarefas mais difíceis.

Por outro lado:

- São mais difíceis de implantar
- Exigem maior infraestrutura
- Consomem mais recursos

Em aplicações simples, um modelo menor pode ser suficiente.

---

## 🔧 Personalização

Alguns modelos permitem:

- Fine-tuning
- Ajustes específicos
- Adaptação ao domínio

Essa capacidade melhora significativamente o desempenho em tarefas especializadas.

---

## 📏 Comprimento de entrada e saída

Cada modelo possui um limite máximo para:

- Entrada (prompt)
- Saída (resposta)

Aplicações que trabalham com documentos longos precisam verificar esse limite antes da escolha.

---

## ⚖️ Considerações sobre IA Responsável

Além do desempenho, deve-se avaliar aspectos responsáveis do modelo.

Exemplos:

- Possíveis vieses
- Risco de desinformação
- Segurança
- Uso indevido
- Dados utilizados no treinamento

---

## 🔌 Implantação e integração

Também é importante analisar a facilidade de integração com a infraestrutura existente.

Devem ser considerados:

- APIs disponíveis
- SDKs
- Compatibilidade com frameworks
- Ferramentas da plataforma

---

# ☁️ Principais Modelos Disponíveis no Amazon Bedrock

---

## 🧠 AI21 Labs — Jurassic-2
<img width="87" height="81" alt="image" src="https://github.com/user-attachments/assets/9c98f92a-bc64-43c0-a19c-8f6e25109984" />

Indicado para:

- Geração de textos
- Resumos
- Perguntas e respostas
- Classificação

Possui foco em aplicações corporativas.

---

## 🟠 Amazon Titan
<img width="91" height="78" alt="image" src="https://github.com/user-attachments/assets/454c8880-1563-4aae-a6ad-386c6be72144" />

Família de modelos criada pela própria AWS.

Tipos disponíveis:

- 📝 Geração de texto
- 🖼️ Geração de imagens
- 📊 Embeddings

Pode ser utilizado diretamente ou personalizado com Fine-tuning.

---

## 🤖 Anthropic Claude 3
<img width="89" height="70" alt="image" src="https://github.com/user-attachments/assets/7d179605-8b3f-44b9-9f9d-09ef6d84ce53" />

Família composta por:

- Haiku
- Sonnet
- Opus

Permite escolher o equilíbrio entre:

- Inteligência
- Velocidade
- Custo

Suporta processamento de texto e visão.

---

## 💬 Cohere Command
<img width="82" height="83" alt="image" src="https://github.com/user-attachments/assets/4e775fd0-5d7b-42e1-8cb1-62400b43b905" />

Especializado em aplicações empresariais.

Utilizado para:

- Chatbots
- Resumos
- Perguntas e respostas
- Extração de informações
- Geração de texto

---

## 🦙 Meta Llama 3
<img width="91" height="67" alt="image" src="https://github.com/user-attachments/assets/d1e75329-f656-47ac-b424-9001e3f8e583" />

Família de LLMs baseada na arquitetura Transformer.

Características:

- Excelente geração de texto
- Contexto coerente
- Grande flexibilidade

Muito utilizada em projetos open source.

---

## 🚀 Mistral Large
<img width="95" height="85" alt="image" src="https://github.com/user-attachments/assets/fac67001-22a2-4883-abd9-e8e78b1ceee9" />

Modelo focado em tarefas complexas.

Excelente para:

- Geração de código
- Agentes
- RAG (Retrieval-Augmented Generation)
- Problemas que exigem raciocínio avançado

---

## 🎨 Stable Diffusion
<img width="78" height="78" alt="image" src="https://github.com/user-attachments/assets/2453c469-fc86-455d-bcc4-140c8f8cfaec" />

Especializado em geração de imagens.

Recebe descrições em texto e produz imagens realistas.

É um dos modelos de geração de imagens mais utilizados atualmente.

---

# 🎯 Escolhendo o Modelo Ideal

Não existe um único modelo "melhor".

O modelo ideal depende do caso de uso.

A escolha deve equilibrar:

- Qualidade
- Velocidade
- Custo
- Responsabilidade
- Recursos computacionais
- Facilidade de integração

Além disso, novos modelos surgem constantemente, tornando importante revisar periodicamente os critérios de seleção.

---

## 🔁 Comparações importantes

---

### Modelo pré-treinado vs modelo desenvolvido do zero

| Modelo pré-treinado | Modelo desenvolvido do zero |
|----------------------|-----------------------------|
| Já possui conhecimento prévio | Aprende tudo durante o treinamento |
| Mais rápido para implementar | Muito mais demorado |
| Menor custo inicial | Alto custo de treinamento |
| Pode ser ajustado (Fine-tuning) | Totalmente personalizado |

---

### Modelos grandes vs modelos pequenos

| Modelos grandes | Modelos pequenos |
|-----------------|------------------|
| Melhor desempenho | Menor desempenho em tarefas complexas |
| Maior custo | Mais baratos |
| Mais memória | Menos memória |
| Maior latência | Menor latência |

---

### Modalidades

| Modalidade | Exemplo |
|------------|----------|
| Texto | Claude, Llama, Jurassic |
| Imagem | Stable Diffusion |
| Embeddings | Amazon Titan Embeddings |
| Multimodal | Claude 3 |

---

## 🧠 Conceitos importantes para prova

- Foundation Model (FM) = modelo de base pré-treinado.
- A seleção do modelo ocorre **após a definição do caso de uso**.
- O caso de uso determina os critérios de seleção.
- Modelos pré-treinados reduzem tempo e custo de desenvolvimento.
- Critérios importantes incluem:
  - Custo
  - Latência
  - Modalidade
  - Tamanho
  - Personalização
  - IA Responsável
- O Amazon Bedrock oferece modelos de diversos provedores.

---

## ⚠️ Pegadinhas comuns

- Modelo maior **não significa** automaticamente melhor para todos os casos.
- O modelo mais barato pode não atender aos requisitos de desempenho.
- Fine-tuning melhora modelos, mas aumenta custos.
- Latência é tão importante quanto qualidade em aplicações em tempo real.
- A escolha do modelo depende do caso de uso, não da popularidade.
- IA responsável também faz parte dos critérios de seleção.

---

## 🔁 Resumo rápido

- Após definir o caso de uso, seleciona-se o Foundation Model.
- Modelos pré-treinados aceleram o desenvolvimento.
- A escolha deve equilibrar custo, desempenho e infraestrutura.
- O Amazon Bedrock reúne modelos de diversos fornecedores.
- Não existe um modelo universalmente melhor; tudo depende da aplicação.

---

## 📌 Status de aprendizado

- [ ] Sei o que é um Foundation Model (FM)
- [ ] Entendo quando utilizar um modelo pré-treinado
- [ ] Conheço os principais critérios de seleção
- [ ] Sei diferenciar modelos grandes e pequenos
- [ ] Conheço os principais modelos disponíveis no Amazon Bedrock
- [ ] Entendo que o caso de uso define a escolha do modelo
