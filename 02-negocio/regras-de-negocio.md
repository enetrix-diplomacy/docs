# Regras de Negócio

## Visão geral

| ID | Regra | Prioridade | Status |
|---|---|---|---|
| RN-001 | Acesso ao sistema | Alta | Aprovada |
| RN-002 | Perfis de acesso | Alta | Em validação |
| RN-003 | Registro de alterações | Média | Proposta |

## RN-001 — Título da regra

**Descrição:**  
O sistema deve...

**Justificativa:**  
Explique por que a regra existe.

**Origem:**  
Área, norma, legislação ou responsável que definiu a regra.

**Aplicação:**  
Indique em quais funcionalidades a regra deve ser aplicada.

**Exceções:**  
Descreva as situações em que a regra não se aplica.

**Requisitos relacionados:**  
RF-001, RF-004.

**Critérios de validação:**

- Dado que...
- Quando...
- Então...

**Status:** Aprovada  
**Responsável:** Área ou pessoa

## RN-001 — Acesso ao sistema

| Campo | Informação |
|---|---|
| **Descrição** | O sistema deve permitir acesso apenas a usuários previamente cadastrados. |
| **Justificativa** | Evitar o acesso de pessoas não autorizadas. |
| **Origem** | Equipe gestora do projeto |
| **Aplicação** | Autenticação e controle de acesso |
| **Exceções** | Não se aplica à página pública inicial. |
| **Requisitos relacionados** | RF-001, RF-002 |
| **Critérios de validação** | Usuário não cadastrado deve ter o acesso recusado. |
| **Prioridade** | Alta |
| **Status** | Aprovada |
| **Responsável** | Equipe de produto |
