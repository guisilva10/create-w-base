# Create W Base - Next.js Starter Kit

<div align="center">

**[English](#-english) | [Portugues](#-portugues)**

</div>

---

# English

A high-performance, opinionated boilerplate for Full Stack applications with **NextAuth v5**, **Prisma**, and **shadcn/ui**.

## Quick Start

```bash
pnpm create w-base my-app
cd my-app
pnpm install
cp .env.example .env
# Fill in your database credentials
pnpm db:generate
pnpm db:push
pnpm dev
```

Access: [http://localhost:3000](http://localhost:3000)

---

## Tech Stack

- **Framework:** [Next.js 16](https://nextjs.org/) (App Router) + React 19
- **Styling:** [Tailwind CSS v4](https://tailwindcss.com/) & [Shadcn UI](https://ui.shadcn.com/)
- **ORM:** [Prisma 7](https://www.prisma.io/)
- **Authentication:** [NextAuth v5](https://authjs.dev/) (Beta)
- **Data Fetching:** [TanStack Query v5](https://tanstack.com/query/latest)
- **Forms:** [React Hook Form](https://react-hook-form.com/) + [Zod](https://zod.dev/)
- **3D Effects:** [Three.js](https://threejs.org/) + React Three Fiber
- **Quality:** Prettier, ESLint & TypeScript

---

## Folder Structure

```plaintext
src/
├── app/                    # Routes, layouts and pages (App Router)
│   ├── (private)/app/      # Authenticated routes
│   ├── (public)/           # Public routes (landing, auth)
│   ├── api/auth/           # NextAuth API handler
│   ├── _components/        # Reusable UI components (shadcn)
│   ├── _hooks/             # Custom hooks
│   └── _lib/               # Utilities
├── features/               # Domain-grouped logic (Auth, etc)
├── providers/              # Context Providers (QueryClient, Theme)
├── services/               # External service clients (Prisma, Auth)
├── types/                  # Global TypeScript definitions
prisma/                     # Database schema and migrations
```

---

## Available Scripts

| Command              | Description                              |
| :------------------- | :--------------------------------------- |
| `pnpm dev`           | Starts the development server.           |
| `pnpm build`         | Builds the application for production.   |
| `pnpm start`         | Starts the server in production mode.    |
| `pnpm lint`          | Runs ESLint verification.                |
| `pnpm db:generate`   | Generates the Prisma Client.             |
| `pnpm db:push`       | Pushes schema to database.               |
| `pnpm db:migrate`    | Runs database migrations.                |

---

## Essential Variables

| Variable              | Description                                              |
| :-------------------- | :------------------------------------------------------- |
| `DATABASE_URL`        | Connection string to your PostgreSQL database.           |
| `AUTH_SECRET`         | Random string for token security (NextAuth).             |
| `SESSION_COOKIE_NAME` | Session cookie name (default: `authjs.session-token`).   |
| `NEXT_PUBLIC_APP_URL` | Base URL of the application.                             |
| `GOOGLE_CLIENT_ID`    | Google OAuth Client ID (optional).                       |
| `GOOGLE_CLIENT_SECRET`| Google OAuth Client Secret (optional).                   |

---

# Portugues

Boilerplate opinativo e de alta performance para aplicacoes Full Stack com **NextAuth v5**, **Prisma** e **shadcn/ui**.

## Inicio Rapido

```bash
pnpm create w-base my-app
cd my-app
pnpm install
cp .env.example .env
# Preencha as credenciais do banco de dados
pnpm db:generate
pnpm db:push
pnpm dev
```

Acesse: [http://localhost:3000](http://localhost:3000)

---

## Tech Stack

- **Framework:** [Next.js 16](https://nextjs.org/) (App Router) + React 19
- **Estilizacao:** [Tailwind CSS v4](https://tailwindcss.com/) & [Shadcn UI](https://ui.shadcn.com/)
- **ORM:** [Prisma 7](https://www.prisma.io/)
- **Autenticacao:** [NextAuth v5](https://authjs.dev/) (Beta)
- **Data Fetching:** [TanStack Query v5](https://tanstack.com/query/latest)
- **Formularios:** [React Hook Form](https://react-hook-form.com/) + [Zod](https://zod.dev/)
- **Efeitos 3D:** [Three.js](https://threejs.org/) + React Three Fiber
- **Qualidade:** Prettier, ESLint & TypeScript

---

## Estrutura de Pastas

```plaintext
src/
├── app/                    # Rotas, layouts e paginas (App Router)
│   ├── (private)/app/      # Rotas autenticadas
│   ├── (public)/           # Rotas publicas (landing, auth)
│   ├── api/auth/           # NextAuth API handler
│   ├── _components/        # Componentes UI reutilizaveis (shadcn)
│   ├── _hooks/             # Hooks personalizados
│   └── _lib/               # Utilitarios
├── features/               # Logica agrupada por dominio (Auth, etc)
├── providers/              # Context Providers (QueryClient, Theme)
├── services/               # Clientes de servicos externos (Prisma, Auth)
├── types/                  # Definicoes globais TypeScript
prisma/                     # Schema do banco e migrations
```

---

## Scripts Disponiveis

| Comando              | Descricao                                |
| :------------------- | :--------------------------------------- |
| `pnpm dev`           | Inicia o servidor de desenvolvimento.    |
| `pnpm build`         | Compila a aplicacao para producao.       |
| `pnpm start`         | Inicia o servidor em modo de producao.   |
| `pnpm lint`          | Executa a verificacao do ESLint.         |
| `pnpm db:generate`   | Gera o Prisma Client.                    |
| `pnpm db:push`       | Envia schema para o banco de dados.      |
| `pnpm db:migrate`    | Executa migrations do banco.             |

---

## Variaveis Essenciais

| Variavel              | Descricao                                               |
| :-------------------- | :------------------------------------------------------ |
| `DATABASE_URL`        | String de conexao com seu banco PostgreSQL.              |
| `AUTH_SECRET`         | String aleatoria para seguranca dos tokens (NextAuth).   |
| `SESSION_COOKIE_NAME` | Nome do cookie de sessao (padrao: `authjs.session-token`).|
| `NEXT_PUBLIC_APP_URL` | URL base da aplicacao.                                   |
| `GOOGLE_CLIENT_ID`    | Client ID do Google OAuth (opcional).                    |
| `GOOGLE_CLIENT_SECRET`| Client Secret do Google OAuth (opcional).                |

---

<div align="center">

Developed with coffee and code by **Willem**

</div>
