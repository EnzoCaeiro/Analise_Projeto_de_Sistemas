https://docs.google.com/document/d/1x05F1FcO4fnLoJRhG9Has47QuRDbZ9oodnn6WrzKIh0/edit?usp=sharing

Modelo do template: https://miro.com/pt/modelos/moscow-matrix-basic/

Atividade realizada em : [Site](https://miro.com/welcomeonboard/T0tRakpjZUdXVjVYNXU3TEtyU29xeWhLZmY1NzltMXFyU04wMGNxbXlMWVNmU1J0Snp2M0ZhY3dlWEx4ck5jSm9mbjY4NlFjOXQxbmZNdEpjWnNZd2xhUUdkSVZvN2VqbDkrV1Q5OXl5TjBHL3RYeUdyQmpaREdTdjBoeVBrUFVBS2NFMDFkcUNFSnM0d3FEN050ekl3PT0hdjE=?share_link_id=99204530044)

# 📋 Projeto de APS [Sistema de Gestão Financeira ]

## Levantamento e Priorização de Requisitos

**Etapa:** Levantamento de Requisitos (Utilizar a ficha dos requisitos levantados) 
**Técnica de Priorização:** MoSCoW  
**Data:** 10/09/2026
**Turma:** D2 - Engenharia de Software  

---

# 👥 1. Identificação do Grupo

| Integrante | Nome |
|---|---|
| 1 |Enzo Caeiro |
| 2 | Victor Alves |
| 3 |Maria Eduarda Moreira |
| 4 |Arthur Santos |
| 5 | Felipe Falcão|

---

# 2. Identificação do Projeto

**Sistema de Gestão Financeira**

**Descrição resumida do projeto:**  

> É um sistema de gestão financeira desenvolvido para gerenciar finanças pessoais de forma simples, segura e organizada. O objetivo é permitir controle centralizado de receitas, despesas, contas e planejamento orçamentário com relatórios e análises detalhadas.

---

# 3. Problema Identificado

## 3.1 Qual problema será resolvido?

> Descreva o problema identificado pelo grupo.  
> Neste momento, concentre-se no problema e não na tecnologia que será utilizada.

**Resposta:**

> A desorganização nas finanças pessoais causada pelo uso de métodos ineficientes (como anotações mentais, cadernos físicos ou planilhas complexas). Essa falta de visibilidade leva ao desconhecimento sobre os "gastos invisíveis", dificultando a poupança e frequentemente resultando em endividamento e estresse.

---

## 3.2 Quem é afetado pelo problema?

> Identifique os principais usuários, grupos ou organizações afetados.

**Resposta:**

> Indivíduos e famílias de diversas faixas de renda que necessitam organizar sua vida financeira cotidiana, mas não possuem conhecimentos avançados em finanças ou planilhas.

---

## 3.3 Como o problema é resolvido atualmente?

> Explique como as pessoas realizam atualmente o processo ou atividade relacionada ao problema.

**Resposta:**

> As pessoas tentam controlar seus gastos utilizando cadernos de anotações informais, planilhas do Excel (que quebram facilmente ou são difíceis de atualizar pelo celular), aplicativos complexos que exigem muito tempo, ou simplesmente não fazem controle algum e confiam apenas no saldo final do banco.

---

## 3.4 Principais dificuldades encontradas

Liste pelo menos três dificuldades observadas.

1. Esquecimento de anotar despesas pequenas do dia a dia pela falta de uma ferramenta prática sempre à mão.
2. Dificuldade em visualizar rapidamente para onde o dinheiro está indo (falta de gráficos ou resumos).
3. Incapacidade de saber se um gasto extra vai estourar o orçamento do mês antes de realizá-lo.

---

# 🎯 4. Objetivo do Projeto

Descreva o resultado que o projeto pretende alcançar.

Utilize como referência:

> **Nosso projeto pretende [resultado] para [stakeholder], contribuindo para [benefício].**

**Objetivo:**

> Nosso projeto pretende entregar um sistema prático e mobile-first de gestão financeira para indivíduos e famílias, contribuindo para a redução do endividamento e da ansiedade através do controle centralizado de receitas, categorização de despesas e planejamento orçamentário.

---

# 👤 5. Stakeholders

Identifique as pessoas, grupos ou organizações que possuem interesse ou participação no sistema.

| ID | Stakeholder | Papel | Necessidade/Interesse | Influência |
|---|---|---|---|---|
| ST01 |Usuário Final |Usuário ativo |Registrar gastos facilmente e ver a saúde financeira |Alta 
| ST02 |Equipe de Desenvolvimento |Construtores |Entregar o sistema funcional e no prazo |Alta |
| ST03 |Prof. Kadidja Valéria |Avaliadora |Avaliar a aplicação da Engenharia de Requisitos |Alta |
| ST04 |Provedor de Nuvem |Infraestrutura |Garantir que o sistema fique hospedado no ar |Baixa |
| ST05 |Instituições Financeiras |Possível Integração (Futuro) |Fornecer dados via Open Finance (fora do escopo atual) |Baixa |

---

## Stakeholder principal

**Stakeholder:**

> Usuário Final (Pessoa Física).

**Por que ele foi considerado o principal stakeholder?**

> Porque o sistema existe exclusivamente para resolver a dor desse usuário. Se a interface não for intuitiva e prática para ele registrar as despesas no dia a dia, o sistema não será adotado, tornando todo o desenvolvimento inútil.

---

# 🗣️ 6. Levantamento de Informações

Registre as principais informações obtidas durante o levantamento.

| Pergunta | Resposta |
|---|---|
| O que o usuário precisa fazer? | Registrar ganhos, anotar gastos diários, ver relatórios e definir limites. |
| Qual problema enfrenta atualmente? | Esquece de anotar gastos e não sabe onde cortá-los. |
| Quais informações precisa consultar? | Saldo atual, gastos por categoria e limites de orçamento disponíveis. |
| Quais informações precisa cadastrar ou alterar? | Transações (valor, data, descrição, categoria) e seu próprio perfil/senha. |
| Quais tarefas são repetitivas? | A inserção diária de pequenos gastos (ex: padaria, transporte, delivery) |
| Quais tarefas consomem mais tempo? | Analisar e somar categorias no fim do mês manualmente. |
| Quais erros acontecem atualmente? | Perder o controle do limite do cartão por não somar os gastos picados. |
| Precisa receber notificações? | Sim, alertas quando estiver próximo de estourar o "teto" de uma categoria. |
| Precisa gerar documentos ou relatórios? | Sim, painéis gráficos (dashboards) mostrando o consumo mensal. |
| Existem informações que precisam ser protegidas? | Sim, todos os dados financeiros e senhas (exige banco de dados seguro). |
| O sistema precisará se comunicar com outros sistemas? | Nesta versão inicial, não. Tudo será inserido manualmente. |
| Existem regras obrigatórias que precisam ser respeitadas? | O usuário só pode ver seus próprios dados (isolamento de segurança). |

---

# 💡 7. Necessidades Identificadas

Antes de escrever os requisitos, registre as necessidades identificadas durante o levantamento.

| ID | Stakeholder | Necessidade Identificada | Problema Relacionado |
|---|---|---|---|
| N01 | ST01 | Cadastrar despesas e receitas de forma rápida. | Preguiça/Esquecimento de anotar gastos diários.|
| N02 | ST02 |Entender onde o dinheiro foi gasto visualmente. | Dificuldade em analisar números em planilhas cruas. | 
| N03 | ST03 |Limitar o quanto pode gastar em certas áreas. | Ficar no vermelho por gastar demais em lazer/delivery. | 
| N04 | ST04 |Ser avisado antes de gastar demais. | Só descobrir que estourou o orçamento quando falta dinheiro. | 
| N05 | ST05 |Acompanhar o progresso para comprar/viajar. | Dificuldade de poupar para metas de longo prazo. | 
| N06 | ST06 |Garantia de que ninguém mais verá seus gastos. | Medo de ter informações financeiras expostas. |
| N07 | ST07 |Agrupar os gastos por áreas da vida. | Receitas e despesas misturadas impossibilitam análise. |
| N08 | ST08 |Usar o sistema facilmente pelo celular na rua. | Planilhas dependem de um computador para funcionar bem. |

---
# ⚙️ 8. Requisitos Funcionais

Os requisitos funcionais representam as funcionalidades e os comportamentos esperados do sistema.

Utilize preferencialmente a estrutura:

> **O sistema deve...**

## Exemplo

**RF01 — Consultar solicitação**

> O sistema deve permitir que o usuário consulte o andamento de suas solicitações.

---

## Requisitos Funcionais do Projeto

| ID | Requisito Funcional | Stakeholder/Fonte | Necessidade | Prioridade |
|---|---|---|---|---|
| RF01 |O sistema deve permitir o cadastro manual de transações (receitas e despesas) contendo valor, data e descrição. |ST01 |N01, N08 |Alta |
| RF02 |O sistema deve permitir a criação e associação de categorias para cada transação (ex: Alimentação, Lazer). |ST01 |N07 |Alta |
| RF03 |O sistema deve gerar gráficos mensais resumindo o total gasto por categoria. |ST01 |N02 |Média |
| RF04 |O sistema deve permitir a definição de um limite de orçamento (teto) para cada categoria. |ST01 |N03 |Média |
| RF05 |O sistema deve emitir um alerta na tela quando o usuário atingir 90% do orçamento estipulado para uma categoria. |ST01 |N04 |Baixa |
| RF06 |O sistema deve permitir o cadastro de metas financeiras com nome, valor alvo e prazo. |ST01 |N05 |Baixa |
| RF07 |O sistema deve gerenciar autenticação de usuários (cadastro, login e recuperação de senha). |ST01 |N06 |Alta|
| RF08 |O sistema deve exibir um extrato completo com o histórico de todas as transações, permitindo filtros por mês. |ST01 |N02 |Alta |

---

# ⭐ 9. Requisitos de Qualidade

Os requisitos de qualidade devem ser escritos de forma clara e, sempre que possível, **mensurável e verificável**.

Evite:

> ❌ O sistema deve ser rápido.

Prefira:

> ✅ O sistema deve apresentar o resultado das consultas em até 2 segundos para 95% das requisições.

---

## Requisitos de Qualidade do Projeto

| ID | Característica de Qualidade | Requisito | Como será verificado? |
|---|---|---|---|
| RQ01 | Desempenho | | |
| RQ02 | Segurança | | |
| RQ03 | Usabilidade/Interação | | |
| RQ04 | Confiabilidade | | |
| RQ05 | Compatibilidade/Portabilidade | | |

---

# 🚧 10. Restrições

Registre as limitações identificadas no projeto.

As restrições podem estar relacionadas a:

- tecnologia;
- prazo;
- orçamento;
- legislação;
- infraestrutura;
- processo;
- recursos disponíveis.

| ID | Restrição | Categoria | Justificativa/Fonte |
|---|---|---|---|
| RES01 |O sistema não terá integração automática com bancos. |Escopo / Complexidade |Definido na matriz MoSCoW ("Won't Have") para garantir a entrega a tempo do projeto APS. |
| RES02 |O sistema deve ser desenvolvido com tecnologias Open Source / Gratuitas. |Orçamento |Projeto acadêmico sem financiamento para licenças de software caras. |
| RES03 |O projeto precisa ser entregue em sua primeira versão até o final do semestre letivo de 2026. |Prazo |Cronograma da disciplina. |

---

# 📜 11. Regras de Negócio

Registre as regras do domínio que precisam ser respeitadas pelo sistema.

## Exemplo

**RN01**

> Somente estudantes regularmente matriculados podem solicitar o serviço acadêmico.

---

| ID | Regra de Negócio | Fonte |
|---|---|---|
| RN01 |O usuário só poderá visualizar, editar ou excluir dados financeiros vinculados ao seu próprio ID de usuário. |ST01 (Segurança) |
| RN02 |Uma transação financeira não pode ser cadastrada sem estar associada a pelo menos uma categoria. |ST01 (Organização) |
| RN03 |Não é possível excluir uma categoria do sistema se houver transações atreladas a ela (exige reatribuição prévia). |Equipe de Desenvolvimento |

---

# 🔗 12. Rastreabilidade Inicial

Relacione as necessidades identificadas aos requisitos correspondentes.

| Necessidade | Stakeholder | Requisito(s) relacionado(s) |
|---|---|---|
| N01 |ST01 |RF01, RQ01 |
| N02 |ST01 |RF03, RF08 |
| N03 |ST01 |RF04 |
| N04 |ST01 |RF05 |
| N05 |ST01 |RF06 |
| N06 |ST01 |RF07, RQ02, RN01 |
| N07 |ST01 |RF02, RN02, RN03 |
| N08 |ST01 |RQ03 |

---

# 🏷️ 13. Priorização dos Requisitos — Técnica MoSCoW

Utilize as seguintes categorias:

| Categoria | Significado |
|---|---|
| 🔴 **M — Must Have** | Requisito indispensável |
| 🟠 **S — Should Have** | Muito importante, mas pode esperar temporariamente |
| 🟢 **C — Could Have** | Desejável se houver tempo e recursos |
| ⚪ **W — Won't Have Now** | Não será implementado nesta entrega |

---

## Matriz de Priorização

| ID | Requisito | MoSCoW | Justificativa |
|---|---|:---:|---|
| RF01 | | M / S / C / W | |
| RF02 | | M / S / C / W | |
| RF03 | | M / S / C / W | |
| RF04 | | M / S / C / W | |
| RF05 | | M / S / C / W | |
| RF06 | | M / S / C / W | |
| RF07 | | M / S / C / W | |
| RF08 | | M / S / C / W | |
| RQ01 | | M / S / C / W | |
| RQ02 | | M / S / C / W | |
| RQ03 | | M / S / C / W | |
| RQ04 | | M / S / C / W | |
| RQ05 | | M / S / C / W | |

---

# 🚀 14. Requisitos da Primeira Versão

Após aplicar a técnica MoSCoW, selecionem os **5 requisitos considerados indispensáveis para a primeira versão**.

| Ordem | ID | Requisito | Por que deve estar na primeira versão? |
|:---:|---|---|---|
| 1 |RF07 |Cadastro e Login |Protege os dados e individualiza a experiência do usuário. |
| 2 |RF01 |Cadastro de Transações |É o coração da aplicação (core business); não existe sistema sem isso. |
| 3 |RF02 |Criação de Categorias |Permite organizar minimamente os dados que foram lançados no RF01. |
| 4 |RF08 |Extrato Completo |O usuário precisa conseguir visualizar o histórico do que acabou de cadastrar. |
| 5 |RQ01 |Interface Rápida (3 cliques) |Garante que a promessa de ser uma ferramenta prática e intuitiva seja cumprida logo na V1. |

---

# ⏭️ 15. Requisitos para Versões Futuras

Selecionem pelo menos três requisitos que poderão ser adiados.

| ID | Requisito | Motivo para adiar | Impacto |
|---|---|---|---|
| | | | |
| | | | |
| | | | |

---

# 🔍 16. Revisão por Pares

**Grupo responsável pela revisão:** __________________________

Registre os problemas identificados durante a revisão.

| ID do Requisito | Problema Encontrado | Sugestão de Melhoria |
|---|---|---|
| | | |
| | | |
| | | |
| | | |

---

# ✅ 17. Checklist de Qualidade dos Requisitos

Antes da entrega, verifique:

- [x] Os requisitos estão completos?
- [x] Os requisitos estão corretos em relação às necessidades?
- [x] Cada requisito representa uma única capacidade ou característica?
- [x] Os requisitos são necessários?
- [x] Os requisitos são viáveis?
- [x] Todos possuem prioridade?
- [x] Termos ambíguos foram eliminados?
- [x] Os requisitos podem ser verificados ou testados?
- [x] A fonte ou stakeholder está identificado?
- [x] As necessidades estão relacionadas aos requisitos?
- [x] Os requisitos de qualidade são mensuráveis sempre que possível?
- [x] As prioridades MoSCoW possuem justificativa?

---

# 💭 18. Reflexão do Grupo

## 18.1 Qual requisito gerou mais discussão durante o levantamento? Por quê?

> A decisão sobre automatizar ou não os gastos via Open Finance. Concluímos que seria inviável para o prazo acadêmico (RES01), por isso o registro precisou se manter manual (RF01), gerando o desafio de fazer isso em até 3 cliques (RQ01) para que não fique chato de usar.


---

## 18.2 Qual necessidade inicialmente parecia simples, mas gerou vários requisitos?

> A necessidade de "entender onde o dinheiro foi gasto" (N02). Isso se desdobrou na necessidade de categorizar transações (RF02), na visão em lista no extrato (RF08) e na geração de gráficos (RF03).


---

## 18.3 O grupo identificou algum requisito implícito durante a discussão?

> Sim. Inicialmente só pensávamos no cadastro de despesas. O requisito implícito foi a segurança e privacidade (RF07 e RN01). Ninguém usará o app se perceber que seus dados financeiros podem vazar ou serem vistos por outras pessoas.


---

## 18.4 Qual requisito foi mais difícil de priorizar utilizando MoSCoW? Por quê?

> Os gráficos mensais (RF03). Embora tragam muito valor para o usuário (quase um Must Have), chegamos à conclusão que para o projeto rodar na primeira versão, listar as despesas no formato extrato cru (RF08) já era o mínimo viável, jogando o gráfico para um Should Have.



---

## 18.5 Houve algum requisito inicialmente considerado Must que mudou de prioridade?

> O limite/teto de orçamentos (RF04). Inicialmente queríamos como obrigatório para resolver a dor do endividamento, mas percebemos que antes de ditar o futuro (orçamento), o app precisa rastrear bem o presente (transações e categorias). Mudou de Must para Should.

---

# 📝 19. Conclusão

Elabore uma breve conclusão apresentando:

- o problema investigado;
- os principais stakeholders;
- as necessidades mais relevantes;
- os requisitos considerados essenciais;
- como a técnica MoSCoW auxiliou na definição da primeira versão.

**Conclusão:**

> O projeto foi motivado pela constante desorganização financeira pessoal devido à ausência de ferramentas simplificadas e acessíveis. Identificamos o "Usuário Final (Pessoa Física)" como stakeholder principal, cujas maiores dores são o esquecimento de registrar os pequenos gastos e o desconhecimento de para onde o dinheiro flui. Para sanar esses problemas, priorizamos requisitos focados em segurança, facilidade de uso (menos de 3 cliques) e categorização clara. O uso da técnica MoSCoW foi fundamental para podar ideias complexas (como integrações automáticas e gráficos avançados) da nossa primeira versão, permitindo que a equipe foque apenas no núcleo do problema: autenticar o usuário, registrar suas transações e exibir um extrato confiável.

---

# 📦 Entregável

O repositório deverá apresentar, no mínimo:

- identificação do projeto e dos integrantes;
- descrição do problema;
- objetivo do projeto;
- stakeholders;
- levantamento das necessidades;
- **8 requisitos funcionais**;
- **5 requisitos de qualidade**;
- **3 restrições**;
- **3 regras de negócio**;
- rastreabilidade entre necessidades e requisitos;
- priorização utilizando **MoSCoW**;
- definição dos requisitos da primeira versão;
- revisão dos requisitos;
- reflexão e conclusão do grupo.

---

# 📚 Referência

REINEHR, Sheila. **Requisitos de Software**. Material de apoio utilizado na disciplina Engenharia de Requisitos.

---

**Disciplina:** Engenharia de Requisitos  
**Projeto:** Levantamento e Priorização de Requisitos  
**Profª Kadidja Valéria**

