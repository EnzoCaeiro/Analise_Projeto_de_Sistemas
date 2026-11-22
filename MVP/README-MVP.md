<div align="center">

# 💸 Sistema de Gestão Financeira

### Anote o gasto. Em 3 toques.

**MVP interativo e responsivo para quem quer controlar o próprio dinheiro sem planilha, sem caderno e sem susto no fim do mês.**

![Status](https://img.shields.io/badge/status-MVP%20funcional-34D399?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Mobile First](https://img.shields.io/badge/mobile--first-320px%2B-0E1B2C?style=for-the-badge)
![Licença](https://img.shields.io/badge/projeto-acadêmico-F2B544?style=for-the-badge)

**Engenharia de Software · UDF Centro Universitário · Turma D2**
**Disciplina:** Análise e Projeto de Sistemas · **Profª** Kadidja Valéria

[📂 Abrir o MVP](./index.html) · [📋 Requisitos](./ProjetoAPS/MoSCow.md) · [🧩 Casos de uso](./Unidade4/ModelagemSistema/CasoDeUsos.md) · [🎨 Lean Canvas](./Unidade4/Lean%20Canvas.png)

</div>

---

## 📖 Sumário

1. [O problema](#-o-problema)
2. [A solução](#-a-solução)
3. [O que o MVP entrega](#-o-que-o-mvp-entrega)
4. [Como testar em 30 segundos](#-como-testar-em-30-segundos)
5. [Requisitos atendidos](#-requisitos-atendidos)
6. [Regras de negócio](#-regras-de-negócio)
7. [Priorização MoSCoW](#-priorização-moscow)
8. [Roadmap](#-roadmap)
9. [Tecnologias](#-tecnologias)
10. [Limitações conhecidas](#-limitações-conhecidas)
11. [Estrutura do repositório](#-estrutura-do-repositório)
12. [Equipe](#-equipe)

---

## 😵 O problema

Muita gente controla o dinheiro no "achismo": anotações mentais, cadernos, planilhas que quebram e que não funcionam bem no celular. O resultado é conhecido:

- 🫥 **Gastos invisíveis:** pequenas despesas do dia a dia que somem com o salário.
- 📉 **Falta de visão:** ninguém sabe rapidamente para onde o dinheiro está indo.
- 😰 **Surpresa no fim do mês:** só se descobre que estourou o orçamento quando o dinheiro acaba.

> *"Como não entendo muito de Excel, preciso de um jeito de anotar meus gastos diários bem rápido pelo celular na rua. Se for demorado, eu acabo esquecendo e chego no fim do mês no vermelho."*
> — Stakeholder ST01, ficha de elicitação REQ-001

## ✨ A solução

Um sistema de gestão financeira pessoal, pensado primeiro para o celular, em que **registrar um gasto leva no máximo 3 toques**. O foco é o usuário leigo: sem termos técnicos, sem fórmulas, sem fricção.

**Nossa proposta de valor:**

> Registre seus gastos em até 3 cliques, entenda para onde vai seu dinheiro e evite surpresas no final do mês.

## 🚀 O que o MVP entrega

### 🔴 Primeira versão (Must Have)

| Funcionalidade | Descrição |
|---|---|
| 🔐 **Cadastro, login e recuperação de senha** | Cada pessoa tem sua conta, e a senha é guardada em hash (SHA-256). |
| ⚡ **Registro rápido de transações** | Receita ou despesa com valor, data, descrição e categoria, em até 3 toques. O botão de tipo define o sinal, então ninguém digita "−". |
| 🏷️ **Categorias personalizadas** | Moradia, Alimentação, Lazer… ou as que você criar. Ao excluir uma categoria em uso, o sistema pede para reatribuir os lançamentos. |
| 🧾 **Extrato completo** | Histórico de tudo que foi lançado, com filtro por mês, edição e exclusão. |
| 📱 **Interface responsiva** | Funciona a partir de 320px, com menu lateral no desktop e barra inferior no celular. |

### 🟠 Já incluído como prévia das próximas versões

| Funcionalidade | Etiqueta no menu | Descrição |
|---|---|---|
| 📊 **Gráfico por categoria** | Painel | Rosca com o percentual gasto em cada categoria no mês. |
| 🎯 **Teto de orçamento** | V1.5 | Limite mensal por categoria com barra de progresso. |
| ⚠️ **Alerta de 90%** | V1.5 | Aviso na tela quando o gasto chega a 90% do teto. |
| 🏁 **Metas financeiras** | V2 | Nome, valor alvo, prazo e acompanhamento do quanto já foi guardado. |

### 🎁 Extras

- 🌓 Tema claro e escuro (respeita a preferência do sistema)
- 🧪 **Conta demo** com dados de dois meses para apresentar em segundos
- ♿ Foco visível no teclado, rótulos de acessibilidade e respeito a `prefers-reduced-motion`

## ⏱️ Como testar em 30 segundos

1. Baixe ou clone o repositório:
   ```bash
   git clone https://github.com/EnzoCaeiro/Analise_Projeto_de_Sistemas.git
   ```
2. Abra o arquivo **`MVP/index.html`** em qualquer navegador moderno. Não precisa instalar nada nem rodar servidor.
3. Clique em **"Explorar com conta demo"** para ver o sistema já com dados.
4. Para ver a regra dos 3 toques: toque em **Novo lançamento**, escolha uma **categoria** e toque em **Salvar**. O contador no topo da tela mostra quantos toques você usou.

> 💡 Teste também no celular, ou redimensione a janela do navegador até 320px de largura.

## ✅ Requisitos atendidos

### Funcionais

| ID | Requisito | Prioridade | No MVP |
|---|---|:---:|:---:|
| RF01 | Cadastro manual de transações (valor, data, descrição) | Alta | ✅ |
| RF02 | Criação e associação de categorias | Alta | ✅ |
| RF03 | Gráficos mensais por categoria | Média | ✅ |
| RF04 | Teto de orçamento por categoria | Média | ✅ |
| RF05 | Alerta ao atingir 90% do teto | Baixa | ✅ |
| RF06 | Metas financeiras (nome, valor alvo, prazo) | Baixa | ✅ |
| RF07 | Autenticação (cadastro, login, recuperação de senha) | Alta | ✅ |
| RF08 | Extrato completo com filtro por mês | Alta | ✅ |

### De qualidade

| ID | Requisito | No MVP |
|---|---|:---:|
| RQ01 | Registro de gasto em no máximo 3 toques a partir da tela inicial | ✅ |
| RQ02 | Senhas guardadas com hash | 🟡 SHA-256 no navegador (bcrypt fica para o back-end) |
| RQ03 | Interface responsiva a partir de 320px | ✅ |
| RQ04 | Carregamento do dashboard em até 2 segundos | ✅ Página única, sem dependências pesadas |
| RQ05 | Integridade de dados (sem transação órfã) | 🟡 Garantida na aplicação; chave estrangeira no banco virá com o back-end |

## 📜 Regras de negócio

| ID | Regra | Como o MVP aplica |
|---|---|---|
| RN01 | Cada usuário só vê e altera os próprios dados | Os dados ficam separados por conta |
| RN02 | Toda transação precisa de categoria | O formulário bloqueia o salvamento e mostra o erro |
| RN03 | Categoria com transações só pode ser excluída com reatribuição | Janela pede a nova categoria antes de excluir |
| RN-003 | O sinal da transação vem da escolha Despesa ou Receita | Botões de tipo no formulário, sem digitar sinal |

## 🧭 Priorização MoSCoW

| Categoria | Requisitos |
|---|---|
| 🔴 **Must have** | RF01, RF02, RF07, RF08, RQ01 |
| 🟠 **Should have** | RF03, RF04 |
| 🟢 **Could have** | RF05, RF06 |
| ⚪ **Won't have agora** | Integração automática com bancos (Open Finance), conforme RES01 |

## 🗺️ Roadmap

- [x] Levantamento e priorização de requisitos (MoSCoW)
- [x] Casos de uso, diagramas UML e Lean Canvas
- [x] **MVP front-end interativo** ← você está aqui
- [ ] Back-end com API e autenticação real (hash bcrypt)
- [ ] Banco de dados relacional (PostgreSQL ou MySQL) com chaves estrangeiras
- [ ] Gráficos interativos avançados e exportação de relatórios
- [ ] Notificações ativas de orçamento
- [ ] Integração Open Finance (versão futura)

## 🛠️ Tecnologias

| Camada | No MVP | Planejado para a versão completa |
|---|---|---|
| Interface | HTML5, CSS3 e JavaScript puro, em um único arquivo | Mesma base, ou React/Vue |
| Armazenamento | `localStorage` do navegador | PostgreSQL ou MySQL |
| Segurança | Web Crypto API (SHA-256) | bcrypt no servidor |
| Lógica de negócio | No navegador | Python (Flask/Django) ou Node.js |
| Arquitetura | Cliente | Em camadas (cliente-servidor) |

Tudo com tecnologias gratuitas e open source (RES02).

## ⚠️ Limitações conhecidas

Para ser transparente sobre o que este MVP **não** é:

- Os dados ficam **apenas no navegador** de cada pessoa. Se limpar o cache ou trocar de aparelho, eles não acompanham.
- A autenticação roda no navegador, então **serve para demonstrar o fluxo, não para proteger dados reais**. Não use dados financeiros verdadeiros nesta versão.
- Não há envio de e-mail na recuperação de senha. Ela é simulada.
- Não existe integração com bancos (fora do escopo, RES01).

## 📁 Estrutura do repositório

```
Analise_Projeto_de_Sistemas/
├── MVP/
│   ├── index.html            ← o MVP (abra no navegador)
│   └── README.md             ← este arquivo
├── ProjetoAPS/
│   ├── README.md             ← visão geral (5W2H)
│   ├── MoSCow.md             ← requisitos e priorização
│   ├── ficha-elicitacao-REQ-001.md
│   └── Documentacao/
├── Unidade2/
│   └── Atividade.md
└── Unidade4/
    ├── Lean Canvas.png
    ├── DocUML/               ← diagramas de objeto e atividade
    └── ModelagemSistema/     ← casos de uso (UC01 a UC14)
```

## 👥 Equipe

<table align="center">
  <tr>
    <td align="center"><a href="https://github.com/EnzoCaeiro"><img src="https://github.com/EnzoCaeiro.png" width="100" alt="Enzo Francisco"/><br/><b>Enzo Francisco</b></a><br/>@EnzoCaeiro</td>
    <td align="center"><a href="https://github.com/arthurnoleto521-hue"><img src="https://github.com/arthurnoleto521-hue.png" width="100" alt="Arthur Santos"/><br/><b>Arthur Santos</b></a><br/>@arthurnoleto521-hue</td>
    <td align="center"><a href="https://github.com/vituadm"><img src="https://github.com/vituadm.png" width="100" alt="Victor Alves"/><br/><b>Victor Alves</b></a><br/>@vituadm</td>
    <td align="center"><a href="https://github.com/moreirafernandesm92-wq"><img src="https://github.com/moreirafernandesm92-wq.png" width="100" alt="Maria Eduarda"/><br/><b>Maria Eduarda</b></a><br/>@moreirafernandesm92-wq</td>
    <td align="center"><a href="https://github.com/2lxpe"><img src="https://github.com/2lxpe.png" width="100" alt="Felipe Falcão"/><br/><b>Felipe Falcão</b></a><br/>@2lxpe</td>
  </tr>
</table>

**Orientação:** Profª Kadidja Valéria · Engenharia de Requisitos / Análise e Projeto de Sistemas
**Instituição:** UDF Centro Universitário · Engenharia de Software · Turma D2

---

## 🤝 Como contribuir

1. Faça um **fork** do projeto
2. Crie uma branch: `git checkout -b feature/nome-da-feature`
3. Faça o commit seguindo [Conventional Commits](https://www.conventionalcommits.org/): `git commit -m "feat: descrição clara"`
4. Envie: `git push origin feature/nome-da-feature`
5. Abra um **Pull Request** com uma descrição detalhada

## 📝 Licença

Projeto acadêmico, sem fins lucrativos.

<div align="center">

**Feito com ☕ e muita discussão de requisitos pela equipe do Sistema de Gestão Financeira**

*Última atualização: novembro de 2026*

</div>
