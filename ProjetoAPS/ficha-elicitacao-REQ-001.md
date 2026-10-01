# Ficha de Elicitação de Requisitos

**Curso:** Engenharia de Software  
**Disciplina:** Análise e Projeto de Sistemas (ProjetoAPS)  
**Instituição:** UDF Centro Universitário  
**Grupo/integrantes:** Enzo Francisco, Arthur Santos, Victor Alves, Maria Eduarda, Felipe Falcão  
**Turma:** D2  **Data:** 30/09/2026  **Versão:** 1.0


## 1. Identificação do projeto

| Campo | Preenchimento |
|---|---|
| Nome do projeto | ProjetoAPS - Sistema de Gestão Financeira |
| Objetivo do projeto | Entregar um sistema prático e mobile-first para controle financeiro, reduzindo a desorganização e a ansiedade através do controle centralizado de receitas, categorização de despesas e planejamento orçamentário. |
| Contexto e escopo | Gestão financeira pessoal e familiar. O escopo da primeira versão contempla o registro rápido de ganhos e gastos, criação de categorias e visualização via extrato, substituindo anotações informais e planilhas complexas. |

## 2. Stakeholder e fonte

| Campo | Preenchimento |
|---|---|
| Stakeholder (nome ou papel) | ST01 - Jovem adulto trabalhador / Chefe de família. |
| Relação com o projeto | Usuário ativo do sistema, principal beneficiário da ferramenta. |
| Contato ou setor (se aplicável) | Pessoas físicas que utilizam smartphone no dia a dia, possuem renda mensal e enfrentam dificuldades em poupar por não terem conhecimentos avançados em finanças ou planilhas de Excel. |
| Técnica e data da elicitação | Análise de problemas com métodos atuais (planilhas/cadernos) e levantamento de necessidades; 10/09/2026. |
| Responsável pelo registro | Equipe de Desenvolvimento |

## 3. Requisito elicitado

| Campo | Preenchimento |
|---|---|
| ID do requisito | REQ-001 (Referente ao RF01 e RQ01) |
| Necessidade relatada pelo stakeholder | "Como não entendo muito de Excel, preciso de um jeito de anotar meus gastos diários (como o pão na padaria ou o Uber) bem rápido pelo celular na rua. Se for demorado, eu acabo esquecendo e chego no fim do mês no vermelho." |
| Descrição consolidada | O sistema deve permitir o cadastro manual de transações (receitas e despesas) informando valor, data, descrição e categoria, exigindo no máximo 3 cliques/toques a partir da tela inicial. |
| Justificativa ou benefício esperado | Sem inserir despesas e receitas, o sistema não tem função. É o coração da aplicação (core business). A exigência de agilidade (3 cliques) garante que o usuário de perfil leigo não abandone o uso diário. |
| Tipo | Funcional e Qualidade (Usabilidade acoplada). |
| Dependências ou dúvidas | Depende do cadastro e autenticação de usuário (RF07) e da existência prévia ou criação simultânea de Categorias (RF02). |

## 4. Regras de negócio

| ID | Regra de negócio relacionada | Fonte ou responsável pela validação |
|---|---|---|
| RN-001 | O usuário só poderá visualizar, editar ou excluir dados financeiros vinculados ao seu próprio ID de usuário (isolamento de segurança). | ST01 (Segurança) / Equipe Dev |
| RN-002 | Uma transação financeira não pode ser cadastrada sem estar associada a pelo menos uma categoria. | ST01 (Organização) / Equipe Dev |
| RN-003 | A interface deve definir automaticamente o sinal da transação (positivo para receita, negativo para despesa) baseado na escolha do usuário, não exigindo digitação de sinais. | Revisão por pares / Equipe Dev |

## 5. Prioridade

**Classificação MoSCoW (marque uma):** 
[X] Must have (essencial)  
[ ] Should have (importante)  
[ ] Could have (desejável)  
[ ] Won't have nesta versão (fora do escopo atual)

**Justificativa da prioridade:** É a funcionalidade base do sistema. Não é possível gerar extratos, gráficos ou controlar o orçamento sem que a entrada de dados (transações) ocorra de maneira funcional e rápida.

## 6. Critérios de aceitação

| ID | Dado/Quando | Então (resultado esperado) | Evidência ou forma de verificação |
|---|---|---|---|
| CA-01 | Dado que o usuário está na tela inicial, Quando ele inserir os dados de uma despesa e confirmar, | Então o sistema deve salvar a transação com sucesso e exibi-la imediatamente no extrato. | Teste funcional na interface e verificação de inserção no Banco de Dados. |
| CA-02 | Dado o formulário de nova transação, Quando o usuário tentar salvar deixando a categoria ou o valor em branco, | Então o sistema deve impedir o cadastro e apresentar uma mensagem clara de erro obrigando o preenchimento. | Teste de validação de campos no front-end. |
| CA-03 | Dado que a regra de agilidade é crucial, Quando o usuário desejar registrar um novo gasto a partir da tela inicial, | Então a conclusão do fluxo inteiro não pode exceder 3 cliques/toques na tela. | Teste de usabilidade rastreando interações (CLI/Analytics). |
| CA-04 | Dado o isolamento de dados, Quando um usuário tentar acessar ou modificar uma transação via API usando um ID diferente do seu, | Então o sistema deve bloquear a ação retornando erro de autorização. | Teste de segurança via endpoint (ex: Postman) forçando IDs de terceiros. |

## 7. Validação e rastreabilidade

| Campo | Preenchimento |
|---|---|
| Situação | [ ] Pendente de validação  [X] Validado  [ ] Necessita revisão |
| Validado por / data | Validação interna pelo grupo (Revisão por Pares) / 10/09/2026 |
| Observações e decisões | A ambiguidade sobre o uso do sinal de menos (-) nas despesas foi resolvida adicionando a RN-003, conforme apontado na revisão. |
| Links relacionados | Origem: RF01, N01, N08, RQ03. Integração com RF02 e RF07. Documento de Requisitos V1. |
