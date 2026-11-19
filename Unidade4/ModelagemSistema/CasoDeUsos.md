# Documentação de Casos de Uso

**Projeto:** ProjetoAPS - Sistema de Gestão Financeira  
**Disciplina:** Análise e Projeto de Sistemas  

---

## 👤 Atores do Sistema

* **Usuário Final (Pessoa Física):** Único ator ativo do sistema nesta versão. Responsável por registrar manualmente suas receitas e despesas, organizar categorias, definir orçamentos e acompanhar relatórios.
  * *Nota de Escopo (RES01):* Instituições financeiras não constam como atores pois a integração automática via Open Finance está fora do escopo da primeira versão.

---

## 📋 Descrição dos Casos de Uso

### Módulo de Acesso (RF07)
| ID | Caso de Uso | Descrição |
| :--- | :--- | :--- |
| **UC01** | Realizar Login | Permite que o usuário autentique-se no sistema com suas credenciais para acessar seus dados privados. |
| **UC02** | Cadastrar Conta | Permite que um novo usuário crie seu perfil de acesso com armazenamento seguro de senha (hash). |
| **UC03** | Recuperar Senha | Permite redefinir a senha de acesso em caso de esquecimento. |

### Módulo de Transações (RF01, RN01, RN02)
| ID | Caso de Uso | Descrição |
| :--- | :--- | :--- |
| **UC04** | Registrar Transação | Permite cadastrar manualmente uma receita ou despesa (valor, data, descrição e categoria obrigatória) em até 3 toques a partir da tela inicial. |
| **UC05** | Editar Transação | Permite alterar os dados de uma transação já registrada pelo próprio usuário. |
| **UC06** | Excluir Transação | Permite remover definitivamente uma transação do histórico do usuário. |

### Módulo de Categorias (RF02, RN03)
| ID | Caso de Uso | Descrição |
| :--- | :--- | :--- |
| **UC07** | Criar Categoria | Permite criar agrupamentos personalizados (ex.: Alimentação, Transporte, Lazer) para classificar as movimentações. |
| **UC08** | Reatribuir/Excluir Categoria | Permite excluir uma categoria existente, exigindo a reatribuição prévia caso existam transações vinculadas a ela. |

### Módulo de Visualização (RF03, RF08)
| ID | Caso de Uso | Descrição |
| :--- | :--- | :--- |
| **UC09** | Consultar Extrato | Exibe a listagem cronológica completa de todas as receitas e despesas lançadas pelo usuário. |
| **UC10** | Filtrar Extrato por Mês | Permite refinar a visualização do extrato selecionando um período mensal específico. |
| **UC11** | Visualizar Gráficos | Gera resumos visuais mensais indicando o percentual e o total gasto por categoria. |

### Módulo de Planejamento (RF04, RF05, RF06)
| ID | Caso de Uso | Descrição |
| :--- | :--- | :--- |
| **UC12** | Definir Teto de Orçamento | Permite estabelecer um limite máximo de gastos mensais para uma determinada categoria. |
| **UC13** | Cadastrar Meta Financeira | Permite registrar objetivos de poupança contendo nome, valor alvo e prazo desejado. |
| **UC14** | Emitir Alerta de 90% | Notifica o usuário na tela automaticamente quando uma nova despesa faz o gasto da categoria atingir 90% do teto definido. |

---

## 🔗 Relacionamentos e Regras Aplicadas

* **Extensões (`<<extend>>`):**
  * **UC07 estende UC04:** Durante o registro de uma transação, caso a categoria desejada ainda não exista, o usuário pode acioná-la opcionalmente para criar uma nova categoria no mesmo fluxo.
  * **UC10 estende UC09:** A aplicação de filtro mensal é uma ação opcional executada a partir da tela de consulta do extrato completo.
  * **UC14 estende UC04:** O disparo do alerta visual ocorre condicionalmente após o registro de uma despesa, apenas se o acumulado atingir 90% do limite estipulado.
* **Pré-condição Global (RN01):** Todos os casos de uso internos (UC04 a UC14) exigem que o usuário esteja previamente autenticado (UC01), garantindo o isolamento estrito dos dados por ID de usuário.
