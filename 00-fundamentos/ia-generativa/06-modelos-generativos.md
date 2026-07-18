# 🎨 Modelos Generativos

## 📌 O que são

Modelos generativos são algoritmos de IA capazes de **criar novos conteúdos** aprendendo padrões presentes nos dados de treinamento.

Eles são a base da **IA Generativa (Generative AI)** e podem produzir diferentes tipos de conteúdo, como:

- Texto
- Imagens
- Áudio
- Vídeos
- Código

📌 Cada arquitetura é mais adequada para determinados tipos de problemas.

---

# 🧠 Principais tipos de modelos

Para a certificação **AWS AI Practitioner**, os principais modelos generativos são:

- Large Language Models (LLMs)
- Modelos Multimodais
- Modelos de Difusão
- GANs (Generative Adversarial Networks)
- VAEs (Variational Autoencoders)

📌 Os **LLMs** são os mais importantes para a prova e já possuem um arquivo específico neste diretório.

---

# 🖼️ Modelos de Difusão (Diffusion Models)

## 📌 O que são

Os **Modelos de Difusão** são arquiteturas especializadas na geração de imagens (e, mais recentemente, vídeos).

Eles aprendem a transformar ruído aleatório em uma imagem coerente.

São amplamente utilizados em modelos modernos de geração de imagens.

---

## ⚙️ Como funcionam

O processo ocorre em duas etapas.

### 1️⃣ Difusão direta (Forward Diffusion)

O modelo adiciona ruído gradualmente a uma imagem até que reste apenas ruído.

<img width="701" height="157" alt="image" src="https://github.com/user-attachments/assets/31df5fa9-4885-44c3-9a08-875c5adc5980" />

---

### 2️⃣ Difusão reversa (Reverse Diffusion)

Depois de aprender esse processo, o modelo faz o caminho inverso:

parte do ruído e remove esse ruído aos poucos até gerar uma nova imagem.

<img width="696" height="154" alt="image" src="https://github.com/user-attachments/assets/4c4cc81e-5b18-4afc-b09a-d7a9eb797bf4" />

---

## 📌 Características

- Excelente qualidade de imagem
- Geração estável
- Alto custo computacional
- Muito utilizado em IA generativa moderna

---

## 💡 Casos de uso

- Geração de imagens
- Edição de imagens
- Geração de arte
- Geração de vídeos

---

# 🖼️ Modelos Multimodais

## 📌 O que são

Modelos multimodais conseguem **processar e gerar diferentes tipos de dados ao mesmo tempo**.

Eles entendem a relação entre diferentes modalidades, como texto, imagem, áudio e vídeo.

---

## 💡 Exemplos

Entrada:

- Texto
- Imagem

Saída:

- Texto
- Nova imagem

---

Outro exemplo:

Entrada:

- Imagem

Saída:

- Descrição da imagem

---

## 📌 Casos de uso

- Descrição automática de imagens
- Perguntas sobre imagens
- Geração de imagens por texto
- Legendagem automática
- Tradução preservando elementos visuais
- Análise de documentos

---

## 📌 Exemplos no Amazon Bedrock

Diversos Foundation Models disponíveis no Bedrock são multimodais, permitindo trabalhar com:

- Texto
- Imagens
- Vídeos

Exemplo:

- Amazon Nova Pro
- Amazon Nova Premier
- Claude (algumas versões)

---

# ⚔️ GANs (Generative Adversarial Networks)

## 📌 O que são

As **GANs (Generative Adversarial Networks)** são modelos compostos por duas redes neurais que competem entre si durante o treinamento.

Uma tenta criar dados falsos.

A outra tenta descobrir se esses dados são reais ou falsos.

---

## ⚙️ Componentes

### Geradora (Generator)

- Cria dados sintéticos
- Recebe ruído aleatório como entrada
- Tenta produzir resultados semelhantes aos dados reais

---

### Discriminadora (Discriminator)

- Recebe dados reais e dados gerados
- Aprende a distinguir quais são verdadeiros

---

## ⚙️ Funcionamento

```text
Ruído
   │
   ▼
Geradora
   │
   ▼
Imagem falsa
   │
   ▼
Discriminadora
   │
   ├── Real
   └── Falsa
```

Durante o treinamento:

- A Geradora tenta enganar a Discriminadora.
- A Discriminadora tenta identificar corretamente os dados falsos.

Esse processo continua até que os dados gerados sejam muito semelhantes aos dados reais.

---

## 📌 Características

- Excelente qualidade de imagem
- Treinamento complexo
- Pode apresentar instabilidade

---

## 💡 Casos de uso

- Geração de rostos
- Restauração de imagens
- Deepfakes
- Super-resolução
- Criação de imagens sintéticas

---

# 🧩 VAEs (Variational Autoencoders)

## 📌 O que são

Os **VAEs (Variational Autoencoders)** são modelos generativos baseados em codificadores automáticos (Autoencoders).

Eles aprendem uma representação compacta dos dados e utilizam essa representação para gerar novos exemplos semelhantes.

---

## ⚙️ Componentes

### Codificador (Encoder)

Transforma os dados em um espaço latente.

---

### Espaço Latente

Representação matemática compacta das principais características dos dados.

---

### Decodificador (Decoder)

Reconstrói os dados a partir do espaço latente.

---

## ⚙️ Funcionamento

```text
Imagem
    │
    ▼
Encoder
    │
    ▼
Espaço Latente
    │
    ▼
Decoder
    │
    ▼
Nova imagem
```

---

## 📌 Características

- Geração mais estável
- Estrutura matemática simples
- Boa representação dos dados

---

## 💡 Casos de uso

- Compressão de dados
- Remoção de ruído
- Geração de imagens
- Detecção de anomalias

---

# 🔁 Comparação entre os modelos

| Modelo | Principal uso | Destaque |
|---------|---------------|----------|
| LLM | Texto | Conversação, geração de texto e código |
| Difusão | Imagens e vídeos | Alta qualidade visual |
| Multimodal | Texto + imagem + vídeo | Trabalha com múltiplas modalidades |
| GAN | Imagens | Geração extremamente realista |
| VAE | Representação de dados | Compressão e geração de dados |

---

# 🧠 O que normalmente aparece na prova

Para a AWS AI Practitioner, normalmente basta saber:

- O que cada arquitetura faz.
- Quando utilizar cada tipo.
- Quais trabalham com imagens.
- Quais trabalham com texto.
- O conceito de modelos multimodais.

📌 Não é esperado conhecer detalhes matemáticos ou arquiteturas internas.

---

# 🧠 Conceitos importantes para prova

- Modelos generativos criam novos conteúdos.
- LLMs são especializados em linguagem natural.
- Modelos de Difusão são amplamente utilizados para geração de imagens.
- Modelos multimodais processam diferentes tipos de dados simultaneamente.
- GANs utilizam uma Geradora e uma Discriminadora competindo durante o treinamento.
- VAEs utilizam um espaço latente para gerar novos dados.

---

# ⚠️ Pegadinhas comuns

- LLM não gera apenas texto: muitos modelos modernos também são multimodais.
- Modelos multimodais não são um tipo específico de algoritmo; são modelos capazes de trabalhar com diferentes modalidades de dados.
- GAN e Modelo de Difusão não são a mesma arquitetura.
- VAEs utilizam Encoder e Decoder, enquanto GANs utilizam Geradora e Discriminadora.

---

# 🔁 Resumo rápido

- **LLM** → linguagem natural
- **Difusão** → geração de imagens e vídeos
- **Multimodal** → texto + imagem + áudio + vídeo
- **GAN** → geradora × discriminadora
- **VAE** → encoder → espaço latente → decoder

---

# 📌 Status de aprendizado

- [ ] Sei o que é um Modelo de Difusão
- [ ] Sei o que é um modelo Multimodal
- [ ] Entendo o conceito de GAN
- [ ] Entendo o conceito de VAE
- [ ] Sei diferenciar os principais modelos generativos
