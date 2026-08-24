
# ETL-XXX — [Título do processo]

| Campo | Informação |
|---|---|
| **Domínio/Módulo** | [área] |
| **Objetivo** | [resultado de negócio produzido] |
| **Tipo de execução** | [Lote / Streaming / Sob demanda] |
| **Periodicidade/Gatilho** | [cron, evento ou ação] |
| **Responsável** | [equipe] |
| **Criticidade** | [Alta / Média / Baixa] |
| **Status** | [Proposto / Implementado / Suspenso / Obsoleto] |

## 1. Escopo

[Descreva quais dados são processados, a finalidade e o que não faz parte deste processo.]

## 2. Fontes de dados

| Fonte | Tipo/Formato | Local/Interface | Credencial | Disponibilidade esperada |
|---|---|---|---|---|
| [sistema] | [API/CSV/JSON/banco] | [referência, sem segredo] | [mecanismo, sem credencial real] | [janela/SLA] |

## 3. Destinos

| Destino | Estrutura | Modo de carga | Chave de identificação |
|---|---|---|---|
| [sistema/tabela] | [tabela/índice/bucket] | [inserção/upsert/substituição] | [chave] |

## 4. Fluxo do processo

1. **Extração:** [como e de onde os dados são obtidos].
2. **Validação inicial:** [estrutura, schema, codificação e obrigatoriedade].
3. **Transformação:** [normalização, conversão, enriquecimento e deduplicação].
4. **Validação final:** [regras de qualidade e consistência].
5. **Carga:** [como os dados são persistidos].
6. **Finalização:** [auditoria, métricas, notificação e disponibilização].

## 5. Mapeamento de dados

| Campo de origem | Tipo de origem | Transformação/Regra | Campo de destino | Tipo de destino | Obrigatório |
|---|---|---|---|---|---|
| `[campo]` | [tipo] | [transformação ou RN-XXX] | `[campo]` | [tipo] | [Sim/Não] |

## 6. Regras de qualidade

| ID | Dimensão | Regra | Limite esperado | Ação em caso de falha |
|---|---|---|---|---|
| DQ-001 | [Completude/validade/unicidade/consistência/atualidade] | [regra verificável] | [percentual ou quantidade] | [rejeitar/quarentenar/alertar] |

## 7. Duplicidade e idempotência

- **Chave de deduplicação:** [campo ou composição].
- **Política para duplicados:** [ignorar, atualizar, rejeitar ou versionar].
- **Reexecução:** [como evitar efeitos duplicados].
- **Carga parcial:** [permitida ou não e como será retomada].

## 8. Tratamento de erros e reprocessamento

| Falha | Comportamento | Número de tentativas | Destino do registro | Notificação |
|---|---|---|---|---|
| [falha] | [interromper/continuar/rejeitar] | [quantidade/intervalo] | [quarentena/log] | [canal/responsável] |

## 9. Monitoramento e auditoria

| Indicador | Métrica | Valor esperado/Alerta |
|---|---|---|
| Registros recebidos | quantidade por execução | [valor/variação] |
| Registros processados | quantidade e percentual | [valor] |
| Registros rejeitados | quantidade e percentual | [limite] |
| Duração | tempo total | [limite] |
| Defasagem dos dados | tempo desde a origem | [limite] |

Registre, no mínimo: identificador da execução, início, fim, origem, quantidades, resultado e referência dos erros. Não registre dados pessoais desnecessários.

## 10. Segurança, privacidade e retenção

- **Dados pessoais/sensíveis:** [quais ou nenhum].
- **Proteção:** [criptografia, mascaramento e controle de acesso].
- **Retenção:** [prazo de dados, arquivos temporários, rejeitados e logs].
- **Descarte:** [procedimento].

## 11. Dependências e operação

- **Dependências anteriores:** [processos/serviços].
- **Processos posteriores:** [consumidores].
- **Janela de execução:** [horário/duração].
- **Timeout:** [valor].
- **Rollback/recuperação:** [procedimento].
- **Runbook:** [link].

## 12. Critérios de aceite do processo

- [ ] [Resultado verificável da execução normal.]
- [ ] [Comportamento verificável diante de dado inválido.]
- [ ] [Comportamento verificável em reexecução.]
- [ ] [Métricas e alertas disponibilizados.]

## 13. Rastreabilidade

- **Regras de negócio:** [RN-XXX]
- **Requisitos:** [RF-XXX / RNF-XXX]
- **Entidades/tabelas:** [identificação]
- **Endpoints:** [API-XXX]
- **Casos de teste:** [CT-XXX]
- **Código/pipeline:** [link]

## 14. Histórico de alterações

| Versão | Data | Responsável | Alteração |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | [nome ou equipe] | Criação do processo |
