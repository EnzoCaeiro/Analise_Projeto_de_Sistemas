# ProjetoAPS - Sistema de Gestão Financeira

## 📋 Visão Geral

ProjetoAPS é um sistema de gestão financeira desenvolvido para gerenciar finanças pessoais e empresariais de forma simples, segura e organizada. O objetivo é permitir controle centralizado de receitas, despesas, contas e planejamento orçamentário com relatórios e análises detalhadas.

---

## ❓ WHAT (O QUÊ)

### Escopo do Projeto

O ProjetoAPS é uma aplicação web/desktop que oferece:

- **Gestão de Contas**: Controle de múltiplas contas bancárias, carteiras e cartões de crédito
- **Registro de Transações**: Categorização automática de receitas e despesas com suporte a tags
- **Parcelamento**: Lançamento e acompanhamento de transações parceladas
- **Orçamento**: Planejamento e monitoramento de limites por categoria e período
- **Relatórios**: Dashboards com fluxo de caixa, análises por categoria e balanço patrimonial
- **Importação/Exportação**: Suporte a arquivos CSV para backup e migração de dados
- **Controle de Acesso**: Perfis de usuário com permissões diferenciadas

---

## 🎯 WHY (POR QUE)

### Motivação e Justificativa

- **Necessidade de Mercado**: Crescente demanda por ferramentas de controle financeiro pessoal e empresarial
- **Educacional**: Projeto acadêmico para aplicar conceitos de engenharia de software, arquitetura e boas práticas
- **Valor Agregado**: Automatização da gestão financeira, redução de erros manuais e maior visibilidade financeira
- **Escalabilidade**: Base sólida para evolução futura com novas funcionalidades (IA, integração bancária, etc.)

---

## 👥 WHO (QUEM)

### Stakeholders

| Persona | Descrição | Necessidades |
|---------|-----------|--------------|
| **Usuário Final** | Pessoa física que deseja gerenciar suas finanças | Interface intuitiva, segurança, relatórios claros |
| **Administrador** | Gerenciador do sistema | Controle total de usuários, auditoria, backups |
| **Desenvolvedor** | Engenheiro de software | Código bem documentado, arquitetura limpa, APIs claras |
| **Instituição Educacional** | Escola/Universidade | Projeto completo, documentação técnica, demonstração de competências |

### Contribuidores

| Nome | Papel | Contato |
|------|-------|---------|
| Enzo Caeiro | Desenvolvedor Principal | [Seu contato] |
|      |      |      |
|      |      |      |
|      |      |      |
|      |      |      |

---

## 🤔 HOW (COMO)

### Arquitetura e Tecnologias

#### Backend
- **Runtime**: Java 11+ (Spring Boot) / Node.js 14+ (Express) / Python 3.8+ (Django)
- **Banco de Dados**: PostgreSQL (produção) / SQLite (desenvolvimento)
- **Autenticação**: JWT / OAuth2
- **Validação**: Hibernate Validator / Joi / Marshmallow

#### Frontend
- **Framework**: React / Vue / Angular
- **Styling**: Tailwind CSS / Bootstrap
- **Estado**: Redux / Vuex / Context API
- **Ferramentas**: Webpack / Vite

#### DevOps
- **Versionamento**: Git & GitHub
- **Containerização**: Docker & Docker Compose
- **CI/CD**: GitHub Actions / GitLab CI
- **Deploy**: Heroku / DigitalOcean / AWS

### Fluxo de Desenvolvimento

```
1. Autenticação → Login JWT
2. Dashboard → Visão geral financeira
3. Contas → CRUD de contas e carteiras
4. Transações → Registro e categorização
5. Relatórios → Análises e gráficos
6. Configurações → Perfis e permissões
```

---

## ⏰ WHEN (QUANDO)

### Cronograma do Projeto

| Fase | Período | Entregas |
|------|---------|----------|
| **Análise & Requisitos** | Semana 1-2 | Documentação de requisitos, UML, casos de uso |
| **Design da Arquitetura** | Semana 3-4 | Diagramas de componentes, design patterns, ERD |
| **Desenvolvimento Backend** | Semana 5-8 | APIs REST, autenticação, lógica de negócio |
| **Desenvolvimento Frontend** | Semana 5-9 | Interface, integração com APIs |
| **Testes & QA** | Semana 10-11 | Testes unitários, integração, aceitação |
| **Deploy & Documentação** | Semana 12-13 | Produção, manuais de usuário, finalizações |

---

## 📁 Estrutura do Projeto

```
ProjetoAPS/
├── README.md                      # Este arquivo
├── .gitignore                     # Exclusões Git
├── docker-compose.yml             # Orquestração de containers
│
├── docs/                          # 📚 Documentação
│   ├── analise_requisitos/        # Requisitos funcionais e não-funcionais
│   ├── diagramas/                 # UML, arquitetura, ERD
│   ├── api/                       # Documentação de APIs (Swagger/OpenAPI)
│   └── guias/                     # Guias de configuração e deployment
│
├── src/                           # 💻 Código-fonte
│   ├── backend/                   # Servidor/API
│   │   ├── config/                # Configurações
│   │   ├── controllers/           # Controladores
│   │   ├── services/              # Lógica de negócio
│   │   ├── repositories/          # Acesso a dados
│   │   ├── models/                # Entidades
│   │   ├── middlewares/           # Middlewares (autenticação, etc)
│   │   └── main.java/.js/.py      # Arquivo principal
│   │
│   └── frontend/                  # Interface do usuário
│       ├── components/            # Componentes reutilizáveis
│       ├── pages/                 # Páginas principais
│       ├── services/              # Chamadas à API
│       ├── styles/                # CSS/SCSS
│       ├── utils/                 # Funções auxiliares
│       └── App.jsx/.vue/.tsx      # Componente raiz
│
├── migrations/                    # 🗄️ Scripts BD
│   ├── init.sql                   # Schema inicial
│   └── seed.sql                   # Dados de exemplo
│
├── testes/                        # ✅ Testes
│   ├── unit/                      # Testes unitários
│   ├── integration/               # Testes de integração
│   ├── e2e/                       # Testes end-to-end
│   └── postman/                   # Coleções Postman
│
└── scripts/                       # 🛠️ Scripts utilitários
    ├── setup.sh                   # Setup inicial
    ├── seed-db.sh                 # Popular BD
    ├── backup.sh                  # Backup automático
    └── deploy.sh                  # Deploy
```

---

## 🚀 Como Executar

### Pré-requisitos

- Git
- Docker & Docker Compose (recomendado)
- OU:
  - Java 11+ / Node.js 14+ / Python 3.8+
  - PostgreSQL 12+
  - npm/yarn (frontend)

### Opção 1: Com Docker (Recomendado)

```bash
# Clone o repositório
git clone https://github.com/EnzoCaeiro/Analise_Projeto_de_Sistemas.git
cd Analise_Projeto_de_Sistemas/ProjetoAPS

# Copie o arquivo de variáveis de ambiente
cp .env.example .env

# Inicie os containers
docker-compose up --build

# Acesse a aplicação
# Frontend: http://localhost:3000
# Backend: http://localhost:8080
# Banco: localhost:5432
```

### Opção 2: Instalação Manual (Java + Spring Boot)

```bash
# Clone e acesse
git clone https://github.com/EnzoCaeiro/Analise_Projeto_de_Sistemas.git
cd Analise_Projeto_de_Sistemas/ProjetoAPS

# Configure variáveis de ambiente
export DATABASE_URL=jdbc:postgresql://localhost:5432/projetoaps
export JWT_SECRET=sua_chave_secreta_aqui
export SPRING_PROFILE_ACTIVE=dev

# Backend
./mvnw clean install
./mvnw spring-boot:run

# Frontend (em outro terminal)
cd src/frontend
npm install
npm run dev
```

### Opção 3: Instalação Manual (Node.js + Express)

```bash
# Backend
cd src/backend
npm install
npm start

# Frontend (em outro terminal)
cd src/frontend
npm install
npm run dev
```

---

## 📡 API REST (Resumo)

### Autenticação
- `POST /api/auth/login` — Login de usuário
- `POST /api/auth/register` — Registro de novo usuário
- `POST /api/auth/refresh` — Renovar token JWT

### Usuários
- `GET /api/users` — Listar usuários (admin)
- `POST /api/users` — Criar usuário
- `GET /api/users/:id` — Detalhes do usuário
- `PUT /api/users/:id` — Atualizar usuário
- `DELETE /api/users/:id` — Deletar usuário

### Contas
- `GET /api/accounts` — Listar contas
- `POST /api/accounts` — Criar conta
- `PUT /api/accounts/:id` — Atualizar conta
- `DELETE /api/accounts/:id` — Deletar conta

### Transações
- `GET /api/transactions` — Listar transações
- `POST /api/transactions` — Criar transação
- `PUT /api/transactions/:id` — Atualizar transação
- `DELETE /api/transactions/:id` — Deletar transação

### Relatórios
- `GET /api/reports/cashflow` — Fluxo de caixa
- `GET /api/reports/by-category` — Despesas por categoria
- `GET /api/reports/balance` — Balanço
- `GET /api/reports/forecast` — Previsão financeira

**Documentação completa**: Ver `docs/api/` (Swagger/OpenAPI)

---

## 🧪 Testes

```bash
# Testes unitários (Backend)
./mvnw test

# Testes unitários (Frontend)
npm run test

# Cobertura de testes
./mvnw test jacoco:report
npm run test:coverage

# Testes E2E (Cypress/Selenium)
npm run test:e2e
```

---

## 📊 Modelagem

### Diagrama Entidade-Relacionamento (ERD)
```
USUÁRIOS ──┐
           ├─→ CONTAS ──┐
PERMISSÕES┘             ├─→ TRANSAÇÕES
                        │
                   CATEGORIAS
                        │
                    ORÇAMENTOS
```

### Casos de Uso Principais
- Autenticar-se no sistema
- Gerenciar contas
- Registrar transações
- Visualizar relatórios
- Exportar dados em CSV

*Diagramas detalhados em `docs/diagramas/`*

---

## 🔒 Segurança

- ✅ Autenticação com JWT/OAuth2
- ✅ Validação de entrada (OWASP Top 10)
- ✅ Criptografia de senhas (bcrypt)
- ✅ HTTPS obrigatório em produção
- ✅ CORS configurado
- ✅ Rate limiting nas APIs
- ✅ Auditoria de operações críticas

---

## 📚 Documentação

- **`docs/analise_requisitos/`** — Especificação funcional
- **`docs/diagramas/`** — UML e arquitetura
- **`docs/api/`** — Documentação de APIs
- **`docs/guias/`** — Setup, deployment e troubleshooting
- **`src/backend/README.md`** — Específico do backend
- **`src/frontend/README.md`** — Específico do frontend

---

## 🤝 Contribuições

Contribuições são bem-vindas! Para contribuir:

1. **Fork** do projeto
2. Criar **branch** da feature: `git checkout -b feature/nome-da-feature`
3. **Commit** suas alterações: `git commit -m "feat: descrição clara"`
4. **Push** para o branch: `git push origin feature/nome-da-feature`
5. Abrir um **Pull Request** com descrição detalhada

### Padrões de Contribuição

- Siga [Conventional Commits](https://www.conventionalcommits.org/)
- Mantenha código com estilo consistente (Prettier, Checkstyle)
- Adicione testes para novas funcionalidades
- Atualize a documentação conforme necessário

---

## 📝 Licença

Projeto acadêmico — Verificar com a instituição a política de licenciamento.

Sugestão: Licença [MIT](LICENSE) ou [Apache 2.0](LICENSE) neste repositório.

---

## 📞 Contato & Suporte

| Canal | Informação |
|-------|-----------|
| **Autor** | Enzo Caeiro |
| **Email** | [Seu email] |
| **GitHub** | [@EnzoCaeiro](https://github.com/EnzoCaeiro) |
| **Issues** | [Reportar bug ou sugerir feature](../../issues) |

---

## 📈 Roadmap

- [ ] MVP com funcionalidades core
- [ ] Integração com bancos reais
- [ ] Mobile app (React Native/Flutter)
- [ ] Inteligência Artificial para recomendações
- [ ] Integração com blockchain para notarização
- [ ] Suporte multi-moeda

---

## 🙏 Agradecimentos

- Universidade/Instituição
- Orientadores e mentores
- Comunidade open-source

---

**Última atualização:** Setembro de 2026  
**Status do Projeto:** Em desenvolvimento 🔄
