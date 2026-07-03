# 🚀 Implantação da Aplicação

<img width="912" height="106" alt="image" src="https://github.com/user-attachments/assets/66a3749c-0a98-46ad-954f-70b3bb8b31e8" />

A fase de **implantação** do ciclo de vida da IA generativa consiste em disponibilizar o modelo para uso em um ambiente real (produção), permitindo que usuários ou outras aplicações utilizem seus recursos.

Nessa etapa, o modelo deixa o ambiente de desenvolvimento e passa a atender requisições reais.

Além de disponibilizar o modelo, essa fase também envolve garantir que a aplicação seja:

- Escalável
- Segura
- Confiável
- Disponível
- Fácil de manter

---

# 🎯 Objetivos da implantação

- Disponibilizar o modelo para uso em produção
- Integrar o modelo à aplicação
- Garantir desempenho adequado
- Proteger os dados utilizados
- Permitir monitoramento contínuo

---

# ⚙️ Principais considerações

## 💰 Custo

Na AWS normalmente paga-se apenas pelos recursos utilizados.

Ao implantar um modelo, devem ser considerados custos como:

- Inferência
- Armazenamento
- Rede
- Recursos computacionais

É importante equilibrar desempenho e custo.

---

## 🌎 Regiões

Nem todos os modelos estão disponíveis em todas as Regiões da AWS.

Antes da implantação, verifique:

- Disponibilidade do modelo
- Latência para os usuários
- Requisitos legais sobre localização dos dados

---

## 📊 Cotas

Cada conta AWS possui limites (quotas) de utilização.

Antes da implantação, confirme se há capacidade suficiente para:

- Número de requisições
- Instâncias
- Recursos computacionais
- Throughput

Caso necessário, pode-se solicitar aumento das cotas.

---

## 🔒 Segurança

A segurança depende do local onde o modelo está sendo executado.

### Modelo hospedado na AWS

Aplica-se o **Modelo de Responsabilidade Compartilhada**.

- AWS protege a infraestrutura.
- O cliente protege seus dados, permissões, identidades e configurações.

---

### Modelo externo

Quando o modelo está fora da AWS, deve-se analisar cuidadosamente:

- Quais dados serão enviados
- Como os dados serão protegidos
- Requisitos de privacidade
- Criptografia
- Conformidade regulatória

---

# 🏗️ Integração com a aplicação

Durante a implantação, o modelo precisa ser integrado ao sistema que fará uso dele.

Essa integração pode ocorrer por meio de:

- APIs REST
- SDKs
- Serviços gerenciados (como Amazon Bedrock)
- Microsserviços

O objetivo é permitir que a aplicação envie prompts ao modelo e receba as respostas de forma transparente.

---

# 📈 Escalabilidade

A infraestrutura deve ser capaz de suportar o aumento da demanda.

Uma boa implantação deve permitir:

- Aumento automático de recursos
- Atendimento simultâneo de vários usuários
- Alta disponibilidade
- Baixa latência

Na AWS isso normalmente é realizado utilizando serviços escaláveis.

---

# 👤 Experiência do usuário

Não basta o modelo gerar boas respostas.

Também é importante que:

- As respostas sejam rápidas
- O sistema seja confiável
- O usuário tenha uma boa experiência durante a interação

Uma resposta extremamente precisa pode perder valor se demorar muito para ser entregue.

---

# 📊 Monitoramento após a implantação

Após entrar em produção, o modelo deve ser continuamente monitorado.

Alguns indicadores importantes incluem:

- Tempo de resposta
- Taxa de erros
- Disponibilidade
- Uso de recursos
- Custos
- Qualidade das respostas

Esse monitoramento permite identificar problemas rapidamente e decidir quando atualizar ou ajustar o modelo.

---

## 🔁 Comparações importantes

---

### Desenvolvimento vs Implantação

| Desenvolvimento | Implantação |
|----------------|------------|
| Treina o modelo | Disponibiliza o modelo para uso |
| Ambiente de testes | Ambiente de produção |
| Ajusta parâmetros | Garante disponibilidade e desempenho |
| Foco em qualidade | Foco em operação |

---

### Modelo hospedado na AWS vs Modelo externo

| AWS | Modelo externo |
|------|---------------|
| Responsabilidade compartilhada | Segurança depende do provedor externo |
| Integração facilitada | Pode exigir integrações adicionais |
| Serviços gerenciados | Maior responsabilidade do cliente |
| Melhor integração com serviços AWS | Avaliar envio de dados para terceiros |

---

## 🧠 Conceitos importantes para prova

- Implantação = disponibilizar o modelo para produção.
- O modelo deve ser integrado à aplicação.
- Escalabilidade garante atendimento ao aumento da demanda.
- Segurança varia conforme onde o modelo está hospedado.
- Na AWS aplica-se o **Modelo de Responsabilidade Compartilhada**.
- O monitoramento continua mesmo após a implantação.

---

## ⚠️ Pegadinhas comuns

- Implantação **não encerra** o ciclo de vida da IA generativa (o monitoramento e as melhorias continuam).
- Um modelo preciso pode gerar má experiência se tiver alta latência.
- Segurança não é responsabilidade exclusiva da AWS.
- Nem todos os modelos estão disponíveis em todas as Regiões.
- Escalabilidade e disponibilidade também fazem parte da implantação.

---

## 🔁 Resumo rápido

- A implantação coloca o modelo em produção.
- É necessário integrar o modelo à aplicação.
- Devem ser considerados custo, segurança, Regiões e cotas.
- A infraestrutura deve ser escalável e confiável.
- Após a implantação, o modelo continua sendo monitorado continuamente.

---

## 📌 Status de aprendizado

- [ ] Entendo o objetivo da implantação
- [ ] Sei quais fatores considerar antes de implantar
- [ ] Entendo o Modelo de Responsabilidade Compartilhada da AWS
- [ ] Sei por que escalabilidade é importante
- [ ] Entendo a importância do monitoramento após a implantação
