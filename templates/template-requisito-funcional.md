# RF-XXX — [Título do requisito funcional]

> Descreva uma capacidade observável do sistema. Não repita regras de negócio: apenas referencie-as.

| Campo | Informação |
|---|---|
| **Módulo** | [Módulo ou funcionalidade] |
| **Ator(es)** | [Perfis que iniciam ou participam] |
| **Prioridade** | [Alta / Média / Baixa] |
| **Status** | [Proposto / Em validação / Aprovado / Implementado / Obsoleto] |
| **Origem** | [Solicitante, história, processo ou documento] |

## 1. Descrição

O sistema deve [capacidade ou comportamento esperado], permitindo que [ator] [objetivo de negócio].

## 2. Pré-condições

- [Estado ou informação necessária antes da execução.]

## 3. Gatilho

[Evento ou ação que inicia o comportamento.]

## 4. Fluxo principal

1. [O ator realiza uma ação.]
2. [O sistema valida ou processa a solicitação.]
3. [O sistema apresenta ou registra o resultado.]

## 5. Fluxos alternativos e exceções

### FA-01 — [Título]

1. [Condição que desvia do fluxo principal.]
2. [Comportamento esperado.]

### FE-01 — [Título da exceção]

1. [Falha ou condição inválida.]
2. [Tratamento e informação apresentada ao usuário.]

## 6. Pós-condições

- **Em caso de sucesso:** [estado resultante].
- **Em caso de falha:** [estado preservado ou tratamento realizado].

## 7. Dados envolvidos

| Dado | Obrigatório | Origem | Validação/Regra |
|---|---|---|---|
| [nome] | [Sim/Não] | [usuário/sistema/integração] | [formato, limite ou RN-XXX] |

## 8. Critérios de aceitação

- [ ] **CA-01:** Dado que [contexto], quando [ação], então [resultado observável].
- [ ] **CA-02:** Dado que [contexto alternativo], quando [ação], então [resultado observável].
- [ ] **CA-03:** Dado que [condição inválida], quando [ação], então [tratamento esperado].

## 9. Rastreabilidade

- **Regras de negócio:** [RN-XXX]
- **Requisitos não funcionais:** [RNF-XXX]
- **Protótipos/telas:** [link ou identificação]
- **Endpoints:** [API-XXX]
- **Casos de teste:** [CT-XXX]
- **Issue/épico:** [link ou identificação]

## 10. Histórico de alterações

| Versão | Data | Responsável | Alteração |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | [nome ou equipe] | Criação do requisito |
