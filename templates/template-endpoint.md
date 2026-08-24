
# API-XXX — [Método] [Caminho do endpoint]

> Mantenha a especificação executável na ferramenta OpenAPI/Swagger. Use este documento para contexto, contrato relevante, regras, exemplos e decisões que não ficam claros apenas no código.

| Campo | Informação |
|---|---|
| **Serviço/Módulo** | [nome] |
| **Finalidade** | [resumo da operação] |
| **Método** | [GET / POST / PUT / PATCH / DELETE] |
| **Caminho** | `/api/v1/[recurso]` |
| **Autenticação** | [Não exigida / Bearer token / OAuth 2.0 / outra] |
| **Perfis autorizados** | [perfis] |
| **Idempotente** | [Sim / Não / Não se aplica] |
| **Status** | [Proposto / Implementado / Obsoleto] |

## 1. Descrição

[Explique o objetivo, o consumidor e o efeito da operação.]

## 2. Regras e permissões

- [RN-XXX — regra aplicada];
- [restrição de escopo, instituição, perfil ou propriedade do recurso].

## 3. Parâmetros

### Parâmetros de caminho

| Nome | Tipo | Obrigatório | Descrição | Exemplo |
|---|---|---|---|---|
| `id` | [UUID/integer/string] | Sim | [descrição] | `[valor]` |

### Parâmetros de consulta

| Nome | Tipo | Obrigatório | Padrão | Validação | Descrição |
|---|---|---|---|---|---|
| `page` | integer | Não | `1` | `>= 1` | Página solicitada |

### Cabeçalhos

| Nome | Obrigatório | Descrição | Exemplo |
|---|---|---|---|
| `Authorization` | Sim | Token de acesso | `Bearer <token>` |

## 4. Corpo da requisição

```json
{
  "campo": "valor"
}
```

| Campo | Tipo | Obrigatório | Validação | Descrição |
|---|---|---|---|---|
| `campo` | string | Sim | [regra] | [descrição] |

## 5. Resposta de sucesso

### `[200/201/204]` — [Descrição]

```json
{
  "id": "00000000-0000-0000-0000-000000000000",
  "campo": "valor"
}
```

## 6. Respostas de erro

| Código HTTP | Código interno | Situação | Tratamento esperado |
|---|---|---|---|
| `400` | `VALIDATION_ERROR` | Dados inválidos | Corrigir os campos indicados |
| `401` | `UNAUTHORIZED` | Autenticação ausente ou inválida | Autenticar novamente |
| `403` | `FORBIDDEN` | Perfil sem permissão | Negar a operação |
| `404` | `NOT_FOUND` | Recurso inexistente | Informar que não foi encontrado |
| `409` | `CONFLICT` | Conflito com o estado atual | Preservar o estado existente |
| `500` | `INTERNAL_ERROR` | Falha inesperada | Registrar correlação sem expor detalhes internos |

### Formato padronizado de erro

```json
{
  "code": "VALIDATION_ERROR",
  "message": "Não foi possível processar a solicitação.",
  "details": [],
  "correlation_id": "00000000-0000-0000-0000-000000000000"
}
```

## 7. Efeitos colaterais

- **Dados alterados:** [entidades/tabelas].
- **Eventos publicados:** [eventos].
- **Serviços externos acionados:** [serviços].
- **Auditoria/logs:** [informações registradas, sem dados sensíveis].

## 8. Requisitos operacionais

- **Paginação:** [padrão e limite máximo].
- **Ordenação:** [campos e padrão].
- **Rate limit:** [limite].
- **Timeout:** [valor].
- **Cache:** [política].

## 9. Segurança e privacidade

[Descreva autorização por recurso, dados pessoais tratados, mascaramento, retenção e cuidados de log. Não registre segredos ou tokens reais.]

## 10. Exemplos de chamada

```bash
curl --request [MÉTODO] \
  --url 'https://[host]/api/v1/[recurso]' \
  --header 'Authorization: Bearer <token>' \
  --header 'Content-Type: application/json'
```

## 11. Rastreabilidade

- **Requisitos funcionais:** [RF-XXX]
- **Regras de negócio:** [RN-XXX]
- **Requisitos não funcionais:** [RNF-XXX]
- **Casos de teste:** [CT-XXX]
- **OpenAPI/Swagger:** [link]
- **Código-fonte:** [link]

## 12. Histórico de alterações

| Versão | Data | Responsável | Alteração |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | [nome ou equipe] | Criação do contrato |
