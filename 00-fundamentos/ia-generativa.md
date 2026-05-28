## 📌 O que é

IA Generativa (Generative AI) é um tipo de inteligência artificial capaz de **criar conteúdo novo** a partir de padrões aprendidos em dados existentes.

<img width="482" height="475" alt="image" src="https://github.com/user-attachments/assets/adb2cd1c-af5b-47cb-a753-61542038b499" />

📌 Diferente do ML tradicional:
- ML → classifica / prevê
- Generative AI → **gera conteúdo**

---

## 🎯 Quando usar

- Quando é necessário **gerar conteúdo automaticamente**
- Para aumentar produtividade
- Para automatizar tarefas criativas

- Ex:
  - Geração de texto (chatbots, emails, resumos)
  - Geração de imagens
  - Geração de código
  - Tradução e reescrita de texto

---

## ⚙️ Como funciona

A IA Generativa é baseada em modelos treinados com grandes volumes de dados:

1. Coleta de grandes datasets  
2. Treinamento de um modelo (geralmente Deep Learning)  
3. Aprendizado de padrões e estruturas  
4. Geração de novos conteúdos com base em entradas (prompts)

📌 Entrada → **Prompt**  
📌 Saída → Conteúdo gerado

---

## 🧠 Conceitos importantes

### 🧱 Modelos de base ou Modelos fundamentais (Foundation Models)
<img width="906" height="367" alt="image" src="https://github.com/user-attachments/assets/bba00897-4f12-43aa-8aaf-fa0e66907f73" />

- Modelos treinados em **grandes volumes de dados genéricos**
- Podem ser adaptados para múltiplas tarefa
- Podem servir como ponto de partida para o desenvolvimento de modelos mais especializados (base da Generative AI moderna)
- Ex:
  - Modelos de linguagem
  - Modelos de imagem

---

### 🔄 Ciclo de vida de Foundation Models (FM Lifecycle)

#### 📥 Seleção de dados (Data Selection)
- Coleta de grandes volumes de dados diversos
- Pode incluir:
  - Texto
  - Imagens
  - Código
- Qualidade dos dados é crítica

📌 Garbage in, garbage out

---

#### 🧠 Pré-treinamento (Pre-training)
- Treinamento inicial em larga escala
- geralmente é usado o meio de aprendizado autossupervisionado, usando a estrutura dos dados para gerar rótulos automaticamente.
- Modelo aprende padrões gerais dos dados (contextos, significados, etc)
- Não é específico para uma tarefa
- Após o pré-treinamento inicial, o modelo pode ser pré-treinado com mais dados (pré-treinamento contínuo)
  - O objetivo é expandir a base de conhecimento do modelo e melhorar sua capacidade de entender e generalizar em diferentes domínios ou tarefas.

📌 Etapa mais cara e computacionalmente intensiva

---

#### ⚙️ Otimização (Optimization / Fine-tuning)
- Ajuste do modelo para casos específicos
- Pode incluir:
  - Fine-tuning com dados específicos
  - Engenharia de prompts
  - Geração aumentada de recuperação (Retrieval-Augmented Generation ou RAG)
  - Ajuste de parâmetros
  - Alinhamento com humanos (RLHF)

📌 Torna o modelo mais útil para aplicações reais

---

#### 📊 Avaliação (Evaluation)
- Mede desempenho do modelo
- Verifica:
  - Precisão
  - Qualidade das respostas
  - Segurança (bias, toxicidade)

📌 Importante para validar antes de produção

---

#### 🚀 Implantação (Deployment)
- Disponibilização do modelo para uso, desde que atenda aos critérios de desempenho desejados
- Pode envolver a integração do modelo com:
  - API
  - Aplicação (chatbot, sistema interno)
  - Outros sistemas de software

📌 Etapa onde começa a gerar valor

---

#### 🔁 Feedback e melhoria contínua (Feedback Loop)
- Coleta de feedback de usuários, especialistas da área e outros stakeholders
- Monitoramento de desempenho
- Atualizações contínuas do modelo
- Pode envolver:
  - Re-treinamento
  - Ajustes de prompts
  - Atualização de dados

---

### 🧠 Modelos de linguagem (LLMs - Large Language Models)

- Modelos focados em linguagem natural
- Capazes de:
  - Gerar texto
  - Responder perguntas
  - Resumir conteúdo
  - Traduzir
- Para funcionar, utilizam, entre outras coisas, tokens, incorporações e vetores
- Ex:
  - Chatbots
  - Assistentes virtuais

---

### 🔤 Tokens

- Unidade básica de texto usada pelo modelo
- Pode ser:
  - Palavra
  - Parte de palavra
  - Símbolo ou caractere individual (ex: .)
  - Frases
  - Etc
- Como exemplo, a frase “Um cachorrinho é para o cachorro como um gatinho é para o gato.” pode ser dividida nos seguintes tokens:
  - “Um” “cachorrinho” “é” “para” “o” “cachorro” “como” “um” “gatinho” “é” “para” “o” “gato”. 
<img width="711" height="124" alt="image" src="https://github.com/user-attachments/assets/6d1602d6-cb0d-477b-86e7-b1754890ab5b" />

📌 Modelos processam texto em tokens, não palavras completas

---

### ↗️ Incorporações e vetores
<img width="433" height="376" alt="image" src="https://github.com/user-attachments/assets/9ee84a67-5284-4f14-9f45-f5b1a9ef924c" />

- São representações numéricas de tokens em que cada token recebe um vetor (uma lista de números) que captura seu significado e os relacionamentos com outros tokens
  - Os vetores são aprendidos durante o processo de treinamento e permitem que o modelo compreenda o contexto e as nuances da linguagem.
- Por exemplo, o vetor de incorporação do token “gato” pode estar próximo aos vetores de “felino” e “gatinho” no espaço de incorporação, indicando que eles estão semanticamente relacionados
  - Dessa forma, o modelo pode entender que “gato” é semelhante a “felino” e “gatinho” sem estar explicitamente programado com essas relações.

---

### 🔎 Modelo de difusão
- É um sistema de arquitetura de aprendizado profundo que começa com ruído puro ou dados aleatórios
- Informações são adicionadas gradualmente até obterem uma saída coerente
- Os modelos de difusão aprendem por meio de um processo de duas etapas de difusão direta e difusão reversa.
  - Difusão direta: o sistema introduz gradualmente uma pequena quantidade de ruído em uma imagem de entrada até que apenas o ruído permaneça
    <img width="701" height="157" alt="image" src="https://github.com/user-attachments/assets/31df5fa9-4885-44c3-9a08-875c5adc5980" />
  - Difusão reversa: Na etapa de difusão reversa subsequente, a imagem ruidosa é gradualmente introduzida na eliminação de ruído até que uma nova imagem seja gerada
    <img width="696" height="154" alt="image" src="https://github.com/user-attachments/assets/4c4cc81e-5b18-4afc-b09a-d7a9eb797bf4" />

---

### 📌 Modelos multimodais
- Podem processar e gerar vários modos de dados simultaneamente
  - Ex: pode receber uma imagem e algum texto como entrada e, em seguida, gerar uma nova imagem e uma legenda descrevendo-a como saída.
- Aprendem como diferentes modalidades, imagens e texto, estão conectadas e podem influenciar umas às outras
- Casos de uso:
  - Automatizar a legendagem de vídeo
  - Criar gráficos com base em instruções de texto
  - Responder perguntas de forma mais inteligente combinando texto e informações visuais
  - Traduzir conteúdo, mantendo os recursos visuais relevantes

---

### ❗ Outros modelos generativos
#### Redes adversárias generativas (GANs)
- São um tipo de modelo generativo que envolve duas redes neurais competindo entre si em uma estrutura de jogo de soma zero. As duas redes são geradoras e discriminadoras
  - Geradora: gera novos dados sintéticos (por exemplo, imagens, texto ou áudio) pegando ruídos aleatórios como entrada e transformando-os em dados que se assemelham à distribuição de dados de treinamento
  - Discriminadora: obtém dados reais do conjunto de treinamento e dados sintéticos gerados pela geradora como entrada. Seu objetivo é distinguir entre os dados reais e os gerados.
- Durante o treinamento, a geradora tenta gerar dados que possam enganar a discriminadora, levando-a a pensar que são reais, enquanto a discriminadora tenta classificar corretamente os dados reais e os gerados.
  - Esse processo contraditório continua até que a geradora produza dados indistinguíveis dos dados reais.

---

#### Codificadores automáticos variacionais (VAEs)
- São um tipo de modelo generativo que combina ideias de codificadores automáticos (um tipo de rede neural) e inferência variacional (uma técnica da estatística bayesiana)
- Consiste em duas partes:
  - Codificadora: pega os dados de entrada (por exemplo, uma imagem) e os mapeia para um espaço latente de menor dimensão, que captura as características essenciais dos dados
  - Decodificadora: pega a representação latente da codificadora e gera uma reconstrução dos dados de entrada originais
- O principal aspecto dos VAEs é que o espaço latente é incentivado a seguir uma distribuição de probabilidade específica (geralmente uma distribuição gaussiana)
  - Isso permite gerar novos dados por meio da amostragem desse espaço latente e da passagem das amostras pela decodificadora
  
---

### 🧩 Engenharia de Prompt (Prompt Engineering)

- Entrada fornecida ao modelo
- Define o comportamento da resposta
- Qualidade do prompt impacta diretamente o resultado. É muito importante para otimização
  - Prompt vago → resposta genérica
  - Prompt detalhado → resposta mais precisa
- Contém os elementos:
  - Instruções: é a tarefa para o FM realizar. É fornecida uma descrição da tarefa ou instruções sobre o desempenho do modelo
  - Contexto: é a informação externa para orientar o modelo
  - Dados de entrada: é a entrada para a qual você deseja obter uma resposta
  - Indicador de saída: é o tipo ou formato de saída

---

### 🧠 Janela de contexto (Context Window)

- Quantidade máxima de tokens que o modelo consegue processar por vez

📌 Limitação importante:
- Contexto muito grande → pode ser truncado

---

### 🔗 Embeddings

- Representações numéricas de dados (vetores)
- Capturam significado semântico

- Ex:
  - Palavras semelhantes → vetores próximos
  - Busca semântica

---

### 🔄 Fine-tuning (Ajuste fino)
- É um processo de aprendizado supervisionado que envolve usar um modelo pré-treinado e adicionar conjuntos de dados menores e específicos
- Tem objetivo de melhorar o modelo de base, tornando-o mais especializado
- Modifica os pesos dos dados para melhor alinhá-los à tarefa.
- Há duas maneias de realizar o ajuste fino:
  - Ajuste fino de instruções: usa exemplos de como o modelo deve responder a uma instrução específica. O ajuste de prompt é um tipo de ajuste fino de instruções
  - Aprendizado por reforço com base no feedback humano (RLHF): fornece dados de feedback humano, resultando em um modelo mais alinhado às preferências humanas

---

### 🔄 Geração aumentada de recuperação (RAG ou Retrieval-Augmented Generation)
- Técnica que fornece dados relevantes ao domínio como contexto para produzir respostas com base nesses dados
- Recupera um pequeno conjunto de documentos relevantes e os usa para fornecer contexto e responder ao prompt do usuário
- Não altera os pesos do modelo de base (diferentemente do ajuste fino)
  - Dados externos (ex: banco de dados)
- Busca informações em tempo real

📌 Mais barato e flexível que fine-tuning

---

### 🎯 Temperatura (Temperature)

- Controla a aleatoriedade da resposta

- Baixa temperatura:
  - Mais determinístico
  - Mais preciso

- Alta temperatura:
  - Mais criativo
  - Mais variado

---

## 💰 Modelo de cobrança (conceitual)

Na AWS (ex: Bedrock):

- Cobrança baseada em:
  - Tokens de entrada (input)
  - Tokens de saída (output)

📌 Mais tokens → maior custo

---

## 🔒 Segurança (conceitual)

- Riscos:
  - Geração de conteúdo incorreto (hallucination)
  - Vazamento de dados sensíveis
  - Bias (viés)

📌 Necessário:
- Controle de acesso
- Validação de saída
- Governança de dados

---

## 🔁 Comparações importantes

---

### ML tradicional vs Generative AI

| ML tradicional | Generative AI |
|---------------|--------------|
| Classifica / prevê | Gera conteúdo |
| Focado em output específico | Focado em criação |
| Menos complexo | Mais complexo |

---

### Fine-tuning vs RAG

| Fine-tuning | RAG |
|------------|-----|
| Treina o modelo | Usa dados externos |
| Mais caro | Mais barato |
| Mais rígido | Mais flexível |
| Atualização difícil | Atualização fácil |

---

### Baixa vs Alta temperatura

| Baixa temperatura | Alta temperatura |
|------------------|-----------------|
| Mais preciso | Mais criativo |
| Menos variação | Mais variação |

---

## 🧠 Conceitos importantes para prova

- Generative AI = **gera conteúdo novo**
- Baseada em:
  - Foundation Models
  - LLMs
- Prompt impacta diretamente a saída
- Tokens são unidade de custo e processamento
- RAG vs Fine-tuning é MUITO cobrado
- Temperatura controla criatividade

---

## ⚠️ Pegadinhas comuns

- Generative AI não garante respostas corretas
- Mais dados ≠ melhor resposta (depende do prompt)
- Fine-tuning não é sempre necessário
- RAG não treina o modelo
- Tokens ≠ palavras

---

## 🔁 Resumo rápido

- Generative AI cria conteúdo (texto, imagem, código)
- Usa modelos grandes (LLMs / Foundation Models)
- Entrada = prompt
- Saída = conteúdo gerado
- Pode usar:
  - Fine-tuning
  - RAG
- Custo baseado em tokens

---

## 📌 Status de aprendizado

- [ ] Entendo o que é Generative AI
- [ ] Sei o que são Foundation Models e LLMs
- [ ] Entendo o papel de prompts
- [ ] Sei a diferença entre Fine-tuning e RAG
- [ ] Entendo o conceito de tokens e contexto
