# Desafio Microsoft Copilot Studio: Fluxo de Conversa Personalizado

## Objetivo
Criar um **Copilot** com fluxo de diálogo personalizado no Microsoft Copilot Studio, utilizando recursos avançados como respostas generativas, integração com fontes de conhecimento e variáveis para personalização.

---

## 📚 Principais Conceitos Aprendidos

### 1. **Tópicos (Topics)**
- **Função:** Estruturar interações específicas (ex.: "Saudação", "Suporte Técnico").
- **Componentes:**
  - **Condições:** Direcionam o fluxo com base em respostas do usuário.
  - **Ações:** Redirecionam para outros tópicos ou executam tarefas (ex.: salvar dados).
  - **Perguntas:** Coletam informações do usuário (ex.: "Qual seu número de pedido?").

### 2. **Variáveis**
- **Tipos:**
  - **Globais:** Acessíveis em todo o fluxo (ex.: `User.Name`).
  - **Locais:** Restritas a um tópico (ex.: `Order.Number`).
- **Uso:** Personalizar respostas e armazenar dados temporários.

### 3. **Respostas Generativas**
- **O que são:** Respostas dinâmicas geradas por IA (ex.: GPT-4) com base em:
  - Contexto da conversa.
  - **Knowledge Sources** (fontes de conhecimento como documentos ou FAQs).
- **Configuração:** Ativadas nas opções de resposta de um tópico.

### 4. **Knowledge Sources**
- **Função:** Bases de dados ou documentos que alimentam a IA para evitar respostas imprecisas.
- **Exemplos:** 
  - Manuais técnicos em PDF.
  - FAQs da empresa.
  - Políticas de atendimento.

### 5. **Fluxo de Diálogo**
- **Estrutura:** Sequência lógica de interações para resolver uma demanda.
- **Exemplo:**
  ```plaintext
  1. Usuário: "Quero cancelar minha assinatura."
  2. Copilot: 
     - Solicita o número da conta → Armazena em variável.
     - Consulta a base de dados → Gera resposta generativa com IA.
     - Oferece opção de transferência para atendente humano.
