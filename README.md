# 💡 Memoteca — Aplicação Angular 14

Projeto desenvolvido durante o curso **"Angular 14: aplique os conceitos e desenvolva seu primeiro CRUD"** da **Alura**.

O **Memoteca** é uma aplicação web para registro, visualização, edição e exclusão de pensamentos, citações e trechos de poesias ou referências favoritas, conectado a uma API REST simulada com `json-server`.

---

## 🚀 Funcionalidades

- **Mural de Pensamentos:** Listagem dinâmica dos pensamentos cadastrados.
- **Cadastro de Novo Pensamento:** Formulário com seleção de modelos visuais e autoria.
- **Edição:** Alteração do conteúdo, autoria ou modelo de pensamentos existentes.
- **Exclusão:** Confirmação e remoção de pensamentos.
- **Integração REST:** Comunicação assíncrona com backend via `HttpClient` e `Observables` (RxJS).

---

## 🛠️ Tecnologias & Conceitos

- **Framework:** [Angular](https://angular.io/) (v14)
- **Linguagem:** TypeScript
- **Reatividade:** RxJS (`Observable`)
- **Estilização:** CSS3 puro e responsivo
- **API Backend:** [JSON Server](https://github.com/typicode/json-server)
- **Conceitos Angular aplicados:**
  - Componentes e Template-Driven forms
  - *Data Binding* (Property Binding, Event Binding e Two-Way Data Binding com `[(ngModel)]`)
  - Diretivas estruturais (`*ngFor`, `*ngIf`) e de atributo (`[ngClass]`)
  - Serviços e Injeção de Dependência (`@Injectable`)
  - Roteamento com `@angular/router` (`AppRoutingModule`)

---

## 📂 Estrutura do Projeto

```text
Alura_Angular/
├── backend/
│   ├── db.json               # Banco de dados simulado
│   └── package.json          # Script para iniciar json-server na porta 3000
│
├── src/
│   ├── app/
│   │   ├── componentes/
│   │   │   ├── cabecalho/    # Header da aplicação
│   │   │   ├── rodape/       # Footer da aplicação
│   │   │   └── pensamentos/
│   │   │       ├── criar-pensamento/
│   │   │       ├── listar-pensamento/
│   │   │       ├── editar-pensamento/
│   │   │       ├── excluir-pensamento/
│   │   │       ├── pensamento/         # Card individual
│   │   │       ├── pensamento.service.ts # Consumo HTTP
│   │   │       └── pensamento.ts       # Interface Model
│   │   ├── app-routing.module.ts
│   │   └── app.module.ts
│   └── assets/imagens/       # Logos e ícones da aplicação
│
├── angular.json
├── package.json
└── tsconfig.json
```

---

## ⚙️ Como Executar

### 1. Pré-requisitos
- [Node.js](https://nodejs.org/) instalado
- [Angular CLI](https://angular.io/cli) instalado globalmente (`npm install -g @angular/cli`)

### 2. Iniciar o Backend (JSON Server)
Em um terminal, acesse a pasta `backend`, instale as dependências e inicie o servidor:
```bash
cd backend
npm install
npm start
```
> O backend rodará em: `http://localhost:3000/pensamentos`

### 3. Iniciar o Frontend (Angular)
Em outro terminal na raiz do projeto, instale as dependências e inicie o servidor de desenvolvimento:
```bash
npm install
ng serve
```
> Acesse a aplicação no seu navegador em: **`http://localhost:4200`**
