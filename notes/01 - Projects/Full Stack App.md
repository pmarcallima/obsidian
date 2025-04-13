# 🗂️ Projeto Full Stack: Gerenciador de Tarefas

Tecnologias:
- **Front-end:** React (Hooks + Context API)
- **Back-end:** Spring Boot (Web, JPA, Security, Validation)
- **Banco de dados:** PostgreSQL (ou H2 para dev)
- **Autenticação:** JWT

---

## ✅ Roteiro de Desenvolvimento (Guia de Etapas)

---

## 🔁 Fase 1 – Preparação

- [x] Criar repositórios: `todo-backend` e `todo-frontend`
- [x] Iniciar projeto Spring Boot (Spring Initializr)
  - [x] Spring Web
  - [x] Spring Security
  - [x] Spring Data JPA
  - [x] PostgreSQL Driver
  - [x] Lombok
  - [x] Validation (Bean Validation)
- [x] Criar estrutura de pacotes:
  - `config/`, `controller/`, `dto/`, `exception/`, `model/`, `repository/`, `security/`, `service/`
- [x] Iniciar projeto React (com Vite ou Create React App)
- [x] Criar estrutura de pastas:
  - `components/`, `pages/`, `services/`, `context/`, `hooks/`, `utils/`
- [ ] Criar arquivos `.gitignore` e `.env` (front e back)
- [ ] Criar `docker-compose.yml` com PostgreSQL (opcional)
- [ ] Usar H2 como banco padrão em profile `dev`

---

## 🔐 Fase 2 – Autenticação

### Back-end:
- [ ] Criar entidade `User` (nome, email, senha)
- [ ] Criar DTOs:
  - `UserLoginRequest`
  - `UserRegisterRequest`
  - `UserResponse`
- [ ] Criptografar senha com `BCryptPasswordEncoder`
- [ ] Configurar Spring Security
- [ ] Criar camada `AuthenticationService`
- [ ] Criar `AuthController`
- [ ] Endpoints:
  - [ ] `POST /register`
  - [ ] `POST /login`
- [ ] Implementar JWT:
  - [ ] Gerar token no login
  - [ ] Criar filtro para autenticação via token
  - [ ] Validar token e injetar usuário autenticado
  - [ ] CORS configurado por ambiente

### Front-end:
- [ ] Criar telas de login e cadastro
- [ ] Fazer requisições à API com `axios`
- [ ] Criar `AuthContext` para armazenar usuário e token
- [ ] Criar hook `useAuth()`
- [ ] Guardar token no `localStorage`
- [ ] Configurar interceptador do `axios` para incluir JWT
- [ ] Proteger rotas privadas com React Router
- [ ] Exibir mensagens com `toast`

---

## 📋 Fase 3 – Tarefas (CRUD)

### Back-end:
- [ ] Criar entidade `Task` (título, descrição, status, data, usuário)
- [ ] Relacionar `Task` com `User` (ManyToOne)
- [ ] Criar DTOs: `TaskRequest`, `TaskResponse`
- [ ] Adicionar paginação no endpoint de listagem
- [ ] Validar propriedade da tarefa (só dono acessa)
- [ ] Endpoints REST:
  - [ ] `GET /tasks` (com paginação e filtros)
  - [ ] `POST /tasks`
  - [ ] `PUT /tasks/{id}`
  - [ ] `DELETE /tasks/{id}`

### Front-end:
- [ ] Criar componentes:
  - Lista de tarefas
  - Formulário de tarefa
- [ ] Criar `TaskService.js` para centralizar chamadas
- [ ] Ações:
  - Criar
  - Editar
  - Excluir
  - Marcar como concluída
- [ ] Atualizar tarefas em tempo real no estado global/contexto

---

## 🧹 Fase 4 – UX, Filtros e Organização

- [ ] Filtro de tarefas (por status, data, ordem)
- [ ] Criar componentes reutilizáveis:
  - `Button`, `Input`, `Modal`, `Loading`
- [ ] Página de perfil do usuário (opcional)
- [ ] Criar `Skeleton Loadings` para dados
- [ ] Adicionar `ToastNotifications`
- [ ] Tratar estados de erro e sucesso nas requisições
- [ ] Separar lógica de requisições em `services/`

---

## 🧪 Fase 5 – Testes e Ajustes

### Back-end:
- [ ] Testes unitários com `JUnit` e `Mockito`
- [ ] Testes de camada com:
  - `@WebMvcTest` para controllers
  - `@DataJpaTest` para repositórios
- [ ] Testar segurança (acesso não autorizado retorna 401)
- [ ] Testar DTOs e validações

### Front-end:
- [ ] Validação de formulários com `Yup` + `React Hook Form`
- [ ] Testes com `React Testing Library`
- [ ] Simular chamadas com `msw` (Mock Service Worker)

---

## 🚀 Fase 6 – Deploy

- [ ] Configurar variáveis de ambiente para produção
- [ ] Gerar build do back-end (`mvn clean install -Pprod`)
- [ ] Deploy da API (Railway, Render ou Heroku)
- [ ] Deploy do Front-end (Vercel ou Netlify)
- [ ] Testar integração final (login + CRUD)

---

## 🎁 Extras (Opcional)

- [ ] Upload de arquivos nas tarefas
- [ ] Confirmação por e-mail no cadastro
- [ ] Dark mode no front-end
- [ ] Logs de ações no back-end
- [ ] Paginação + ordenação dinâmica nas tarefas
- [ ] Exportar tarefas em PDF/CSV

