# ⚖️ Compensações de Modelos de IA

Ao desenvolver sistemas de IA, nem sempre é possível maximizar todas as características desejadas ao mesmo tempo. Muitas vezes é necessário encontrar um equilíbrio entre fatores como interpretabilidade, explicabilidade, transparência, proteção, desempenho e controlabilidade.

## 🔍 Interpretabilidade x Explicabilidade

Embora os termos sejam parecidos, eles possuem significados diferentes.

### Interpretabilidade

A interpretabilidade é a capacidade de compreender diretamente o funcionamento interno do modelo.

Ela responde às perguntas:

- Como o modelo chegou ao resultado?
- Quais variáveis influenciaram a decisão?
- Qual o peso de cada atributo?

Modelos interpretáveis permitem acesso direto à sua lógica interna.

### Exemplo

Um economista utiliza uma regressão linear para prever a inflação.

Como os coeficientes da regressão são visíveis, ele consegue entender exatamente como cada variável influencia o resultado.

### Explicabilidade

A explicabilidade consiste em explicar o comportamento do modelo de forma compreensível para humanos, mesmo quando seu funcionamento interno é complexo.

Ela responde à pergunta:

- Por que o modelo produziu determinado resultado?

A explicabilidade é especialmente importante para modelos complexos e de caixa-preta.

### Exemplo

Uma empresa de mídia utiliza uma rede neural para classificar notícias.

Embora não consiga visualizar diretamente a lógica interna do modelo, ela usa técnicas de explicação para descobrir que artigos de negócios estão sendo classificados como esportes devido à presença de nomes de organizações esportivas.

## ⚖️ Compensação entre Interpretabilidade e Desempenho

Existe uma relação comum entre interpretabilidade e desempenho.

<img width="918" height="516" alt="image" src="https://github.com/user-attachments/assets/12d0807f-b090-4606-8570-00bad991bc36" />


### Modelos mais interpretáveis

Exemplos:

- Regressão linear
- Árvores de decisão simples

Vantagens:

- Fácil compreensão
- Alta transparência
- Facilidade de auditoria

Desvantagens:

- Podem apresentar menor precisão em problemas complexos

### Modelos mais complexos

Exemplos:

- Redes neurais profundas
- Grandes modelos de linguagem (LLMs)

Vantagens:

- Maior capacidade de aprendizado
- Melhor desempenho em tarefas complexas

Desvantagens:

- Menor interpretabilidade
- Funcionamento interno difícil de compreender

### Regra prática

Quanto maior a interpretabilidade, normalmente menor a complexidade do modelo.

Quanto maior a complexidade, normalmente menor a interpretabilidade.

Nesse cenário, técnicas de explicabilidade tornam-se essenciais.

## 🛡️ Compensação entre Proteção e Transparência

A proteção busca reduzir riscos e evitar danos causados pelo sistema de IA.

A transparência busca tornar o funcionamento do sistema mais visível.

Esses objetivos podem entrar em conflito.

### Precisão

Modelos complexos geralmente são:

- Mais precisos
- Menos transparentes

Modelos simples geralmente são:

- Mais transparentes
- Menos precisos

### Privacidade

Técnicas de preservação de privacidade, como:

- Privacidade diferencial (Differential Privacy)

ajudam a proteger dados sensíveis.

Por outro lado, podem dificultar a análise e auditoria do modelo.

### Proteção

Filtros de segurança e mecanismos de bloqueio podem impedir respostas inadequadas.

Entretanto, também podem ocultar parte do raciocínio utilizado pelo modelo.

### Segurança

Ambientes altamente protegidos podem:

- Aumentar a segurança
- Reduzir a capacidade de auditoria externa

## 🎛️ Controlabilidade do Modelo

A controlabilidade é a capacidade de influenciar o comportamento do modelo.

Ela mede o quanto é possível modificar as previsões alterando:

- Dados de treinamento
- Restrições do treinamento
- Exemplos fornecidos ao modelo

### Benefícios

Maior controlabilidade permite:

- Reduzir vieses
- Corrigir comportamentos indesejados
- Melhorar a transparência
- Facilitar a depuração

### Relação com a arquitetura

Modelos simples tendem a ser mais controláveis.

Exemplos:

- Regressão linear
- Árvores de decisão

Modelos complexos tendem a ser menos controláveis.

Exemplos:

- Redes neurais profundas
- Grandes modelos de linguagem

## 🔧 Como aumentar a controlabilidade

Algumas técnicas incluem:

### Aumento de dados (Data Augmentation)

Adicionar novos exemplos para direcionar o aprendizado do modelo.

### Balanceamento de dados

Reduzir vieses presentes no conjunto de treinamento.

### Restrições de treinamento

Aplicar regras durante o treinamento para limitar comportamentos indesejados.

### Testes de comportamento

Verificar se alterações nos dados produzem mudanças coerentes nas previsões.

## 📝 Resumo para a prova

- Interpretabilidade é entender diretamente o funcionamento interno do modelo.
- Explicabilidade é explicar o comportamento do modelo em linguagem compreensível.
- Modelos simples possuem maior interpretabilidade.
- Modelos complexos geralmente possuem melhor desempenho, porém menor interpretabilidade.
- Transparência e proteção precisam ser equilibradas.
- Técnicas de privacidade podem reduzir a transparência.
- A controlabilidade mede o quanto é possível influenciar o comportamento do modelo.
- Modelos mais controláveis facilitam a correção de vieses e a depuração.
- Data augmentation, balanceamento de dados e restrições de treinamento ajudam a aumentar a controlabilidade.
