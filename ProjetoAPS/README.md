# ProjetoAPS - Sistema de gestão financeira 

## Descrição

ProjetoAPS é um sistema de gestão financeira desenvolvido para gerenciar as finanças pessoais e empresariais de forma simples, segura e organizada. O objetivo é permitir controle de receitas, despesas, orçamentos e relatórios, ajudando usuários a tomar decisões financeiras baseadas em dados.

## Funcionalidades Principais

- Cadastro e autenticação de usuários
- Gerenciamento de contas (bancos, carteiras, cartões)
- Registro de transações: receitas e despesas com categorias e tags
- Lançamento e acompanhamento de parcelas
- Planejamento orçamentário por categoria e período
- Relatórios e gráficos (fluxo de caixa, despesas por categoria, balanço)
- Importação/Exportação de dados (CSV)
- Backup e restauração
- Perfis de usuário com permissões (usuário, administrador)

## Tecnologias (sugestão)

- Backend: Java (Spring Boot) / Node.js (Express) / Python (Django) — escolha conforme o curso
- Banco de Dados: PostgreSQL / MySQL / SQLite (para desenvolvimento)
- Frontend: React / Vue / Angular / Aplicação Desktop com Electron
- Autenticação: JWT / OAuth2
- Ferramentas: Git, Docker (opcional)

## Estrutura do Projeto

```
ProjetoAPS/
├── README.md                 # Este arquivo
├── docs/                     # Documentação do projeto (requisitos, casos de uso)
├── src/                      # Código-fonte
│   ├── backend/              # Código do servidor
│   └── frontend/             # Código da interface do usuário
├── migrations/               # Scripts de migração do BD
├── testes/                   # Testes unitários e de integração
└── scripts/                  # Scripts úteis (seed, import, export)
```

## Requisitos

- Java 11+ ou Node 14+/Python 3.8+ (dependendo da stack escolhida)
- PostgreSQL ou outro SGBD compatível
- Git
- Node.js e npm/yarn (se houver frontend em JS)

## Como executar (exemplo genérico)

1. Clone o repositório

```bash
git clone https://github.com/EnzoCaeiro/Analise_Projeto_de_Sistemas.git
cd Analise_Projeto_de_Sistemas/ProjetoAPS
```

2. Configurar variáveis de ambiente (ex.: DATABASE_URL, JWT_SECRET)

3. Executar o backend

- Exemplo com Spring Boot:

```bash
./mvnw spring-boot:run
```

- Exemplo com Node.js:

```bash
npm install
npm start
```

4. Executar o frontend (se houver)

```bash
cd frontend
npm install
npm run dev
```

## API (exemplo resumido)

- POST /api/auth/login — autenticar usuário
- POST /api/users — cadastrar usuário (admin)
- GET /api/accounts — listar contas
- POST /api/transactions — criar transação
- GET /api/reports/cashflow — relatório de fluxo de caixa

(Detalhar rotas e contratos na documentação técnica em docs/)

## Modelagem e Artefatos

- Diagramas UML: casos de uso, classes, sequência e componentes
- Requisitos funcionais e não funcionais em docs/analise_requisitos/
- Planos de teste em testes/

## Contribuições

Contribuições são bem-vindas. Para contribuir:

1. Fork do projeto
2. Criar branch com a feature: feature/nome-da-feature
3. Abrir Pull Request descrevendo as alterações

## Licença

Projeto acadêmico — verificar com a instituição a política de licenciamento. Se desejar, adicione uma licença (ex: MIT) neste repositório.

## Contato

**Autor:** Enzo Caeiro


**Última atualização:** Setembro de 2026
