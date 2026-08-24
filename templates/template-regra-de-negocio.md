# RN-XXX — [Título da regra de negócio]

> Substitua os campos entre colchetes e remova todas as orientações antes da aprovação.

| Campo | Informação |
|---|---|
| **Domínio/Módulo** | [Área do negócio à qual a regra pertence] |
| **Categoria** | [Elegibilidade / autorização / validação / cálculo / classificação / prazo / transição de estado / integridade / outra] |
| **Prioridade** | [Alta / Média / Baixa] |
| **Status** | [Proposta / Em validação / Aprovada / Obsoleta] |
| **Responsável pela validação** | [Pessoa, papel ou área de negócio] |

## 1. Regra

[Declare objetivamente a política, restrição, cálculo ou decisão do negócio. Prefira uma regra que continue válida mesmo que o processo seja executado sem o sistema.]

## 2. Justificativa

[Explique por que a regra existe e qual problema, risco, política ou obrigação ela atende.]

## 3. Condições de aplicação

A regra se aplica quando:

- [condição 1];
- [condição 2].

## 4. Resultado ou consequência

[Descreva o resultado esperado quando as condições forem atendidas e, se necessário, quando não forem atendidas.]

## 5. Exceções

- [Exceção e tratamento correspondente.]
- Não há exceções conhecidas. <!-- Mantenha apenas se aplicável. -->

## 6. Exemplos

### Exemplo válido

[Apresente dados concretos e o resultado esperado.]

### Exemplo inválido ou caso-limite

[Apresente uma situação que viole a regra ou esteja no seu limite e informe a consequência.]

## 7. Tabela de decisão ou transição de estado

<!-- Use somente se a regra combinar múltiplas condições ou estados. -->

| Condição/Estado atual | Condição adicional/Ação | Resultado/Novo estado |
|---|---|---|
| [valor] | [valor] | [resultado] |

## 8. Origem

- **Fonte:** [legislação, norma, processo, reunião, especialista ou documento]
- **Referência:** [link, seção ou identificação]
- **Data da validação:** [AAAA-MM-DD]

## 9. Rastreabilidade

- **Requisitos funcionais:** [RF-XXX]
- **Requisitos não funcionais:** [RNF-XXX]
- **Dados/entidades:** [entidades ou campos afetados]
- **Endpoints/processos:** [API-XXX / ETL-XXX]
- **Casos de teste:** [CT-XXX]

## 10. Histórico de alterações

| Versão | Data | Responsável | Alteração |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | [nome ou equipe] | Criação da regra |

