# 🚀 Desafio Técnico — LeadLoop CRM Challenge

## 🧠 Contexto

A empresa fictícia **LeadLoop** está desenvolvendo um **CRM interno simples** para sua equipe de vendas acompanhar leads e sua evolução até se tornarem clientes. O objetivo é ter uma **aplicação fullstack (API + SPA)** onde seja possível **cadastrar, editar, listar e deletar contatos** e acompanhar o estágio de cada lead.

---

## 🎯 Objetivo

Construir uma aplicação fullstack com:

- **API em Ruby on Rails (modo API-only)**  
- **Frontend SPA em React**, utilizando [`shadcn/ui`](https://ui.shadcn.com/) (ou não, dependendo do requisito escolhido)

A aplicação deve permitir:

1. Criar, editar, excluir e visualizar **leads (contatos)** com os campos:
   - `full_name`
   - `email`
   - `phone`
   - `status` (enum: `"cold"`, `"warm"`, `"client"`)
   - `created_at` (autogerado)

2. Uma **tela de listagem** com:
   - Busca por **nome, email ou telefone**
   - Exibição do **status**
   - Um componente (ou filtro) para **filtrar por status**

---

## 🧩 Requisitos Técnicos

- Ruby on Rails (última versão estável) - API-only
- React 18+ 
- Lib de UI: [`shadcn/ui`](https://ui.shadcn.com/) (a menos que opte por criar sua própria)
- Código limpo, com organização de pastas, componentes reutilizáveis e boas práticas
- Comunicação com API + tratamento de loading e erros
- Fique à vontade para escolher o que vai usar com o React em termos de build, framework, etc.

---

## ✅ Funcionalidades Esperadas

### 🔙 Backend (Rails API)

- CRUD completo para o modelo **Lead**
- Enum `status`: `"cold"`, `"warm"`, `"client"`
- Busca por query string (`name`, `email`, `phone`)
- Serialização dos dados com uso opcional de `active_model_serializers`

### 🔜 Frontend (React SPA)

- Página de listagem com:
  - Campo de busca (nome/email/telefone)
  - Filtro por status (se selecionado como requisito)
  - Tabela ou cards com dados dos leads
  - Ações de edição e exclusão
- Página/formulário para criação e edição
- Feedback visual (loading, erros, etc.)

---

## 🔧 Pré-Requisitos (Escolha pelo menos **2**)

- [ ] Escrever testes automatizados na UI (ex: Vitest, Testing Library, Cypress)
- [ ] Usar **TypeScript** no frontend
- [ ] Criar um componente em React para **filtrar por estágio/status**
- [ ] Criar a UI **do zero**, sem utilizar `shadcn/ui`
- [ ] Utilizar [`active_model_serializers`](https://github.com/rails-api/active_model_serializers) no backend
- [ ] Implementar autenticação para múltiplos usuários (ex: Devise + JWT)

---

## 📁 Entrega

- Crie um repositório **privado no GitHub** com o nome:  
  **`LeadLoop-crm-challenge`**
- Adicione o usuário **`ibftcorp`** como colaborador **apenas quando o desafio estiver finalizado**
- Crie um arquivo chamado **`DECISIONS.md`** explicando:
  - Quais tecnologias/libraries foram usadas
  - Como você estruturou o projeto (frontend/backend)
  - Quais requisitos extras você escolheu e por quê
  - Como rodar o projeto localmente (instruções claras)
  - Como rodar os testes (se houver)
- Todo o código deve estar em **inglês** (variáveis, comentários, commits, etc.)

---

## ⏱ Tempo Estimado

Entre **4 e 6 horas**. Faça o melhor uso possível do tempo disponível, priorizando clareza, organização e entrega funcional. Não tem problema se quiser gastar mais tempo.

---

## 🧐 Critérios de Avaliação

- Clareza e organização do código
- Qualidade da API e modelagem
- Uso correto do React com boas práticas
- Uso correto dos padrões Rails
- Estrutura dos componentes e da UI
- Validações, loading e tratamento de erros
- Justificativas técnicas no `DECISIONS.md`

---

Boa sorte! 🍀 Qualquer dúvida sobre requisitos implícitos, **faça suposições e documente no `DECISIONS.md`**.
