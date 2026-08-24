> Não é necessário documentar individualmente todo componente visual.
> O template-componente-frontend.md deve ser usado somente para componentes reutilizáveis, complexos ou que tenham regras relevantes,
> como tabelas, filtros, formulários, mapas e controles de permissão.
> 
# FE-XXX — [Nome da tela ou funcionalidade]

> Documente o comportamento da interface sem repetir integralmente os
> requisitos e as regras de negócio. Use a rastreabilidade para referenciá-los.

| Campo | Informação |
|---|---|
| **Módulo** | [Módulo ao qual pertence] |
| **Rota** | `/[caminho]` |
| **Tipo** | [Página / Modal / Fluxo / Formulário / Dashboard] |
| **Perfis autorizados** | [Perfis] |
| **Responsável** | [Pessoa ou equipe] |
| **Status** | [Proposta / Em desenvolvimento / Implementada / Obsoleta] |

## 1. Objetivo

[Explique para que serve a interface e qual necessidade do usuário ela atende.]

## 2. Usuários e permissões

| Perfil | Pode visualizar | Pode incluir | Pode editar | Pode excluir |
|---|---|---|---|---|
| [Perfil] | [Sim/Não] | [Sim/Não] | [Sim/Não] | [Sim/Não] |

## 3. Acesso e navegação

- **Rota de acesso:** `[rota]`
- **Origem da navegação:** [menu, página ou ação]
- **Destino após conclusão:** [rota ou estado]
- **Breadcrumb:** [estrutura]
- **Parâmetros da rota:** [parâmetros ou “Não se aplica”]

## 4. Estrutura da interface

| Área/Elemento | Tipo | Finalidade | Visibilidade |
|---|---|---|---|
| [Nome] | [Campo/Botão/Tabela/Card/Modal] | [Descrição] | [Condição] |

## 5. Campos

| Campo | Tipo | Obrigatório | Formato/Limite | Valor inicial | Validação |
|---|---|---|---|---|---|
| [Nome] | [Texto/Seleção/Data] | [Sim/Não] | [Regra] | [Valor] | [RN-XXX ou validação] |

## 6. Ações disponíveis

| Ação | Elemento | Condição de habilitação | Resultado |
|---|---|---|---|
| [Salvar] | [Botão] | [Condição] | [Comportamento] |

## 7. Estados da interface

### Estado inicial

[Descreva o que é apresentado antes de qualquer interação.]

### Carregamento

[Descreva indicador de carregamento e bloqueio de ações.]

### Sem dados

[Descreva mensagem e ação disponível.]

### Sucesso

[Descreva confirmação, redirecionamento ou atualização.]

### Erro

[Descreva mensagem, preservação dos dados e possibilidade de nova tentativa.]

### Sem permissão

[Descreva o comportamento para usuário não autorizado.]

### Indisponibilidade parcial

[Descreva o comportamento quando somente parte dos dados não estiver disponível.]

## 8. Fluxo principal

1. O usuário [ação].
2. A interface [resposta].
3. O front-end solicita [operação].
4. A interface apresenta [resultado].

## 9. Fluxos alternativos e exceções

### FA-01 — [Título]

1. [Condição alternativa.]
2. [Comportamento esperado.]

### FE-01 — [Título]

1. [Falha.]
2. [Tratamento apresentado ao usuário.]

## 10. Integrações com APIs

| Operação | Endpoint | Momento da chamada | Tratamento de sucesso | Tratamento de erro |
|---|---|---|---|---|
| [Consultar] | [API-XXX] | [Ao abrir a página] | [Comportamento] | [Comportamento] |

## 11. Regras de apresentação

- [Formatação de datas, valores ou textos.]
- [Ordenação padrão.]
- [Paginação.]
- [Máscaras.]
- [Condições de exibição.]

## 12. Validações

| Validação | Momento | Mensagem apresentada | Referência |
|---|---|---|---|
| [Descrição] | [Ao sair do campo/Ao enviar] | [Mensagem] | [RN-XXX/RF-XXX] |

## 13. Responsividade

| Dispositivo/Largura | Comportamento esperado |
|---|---|
| Desktop | [Comportamento] |
| Tablet | [Comportamento] |
| Celular | [Comportamento] |

## 14. Acessibilidade

- [ ] Navegação completa por teclado.
- [ ] Ordem de foco coerente.
- [ ] Rótulos associados aos campos.
- [ ] Mensagens de erro identificáveis por tecnologias assistivas.
- [ ] Contraste adequado.
- [ ] Elementos não dependem exclusivamente de cor.
- [ ] Componentes dinâmicos informam mudanças de estado.

## 15. Segurança e privacidade

- **Dados pessoais apresentados:** [dados ou “Nenhum”].
- **Dados mascarados:** [dados e regra].
- **Armazenamento no navegador:** [localStorage, sessionStorage, cookie ou nenhum].
- **Proteção de rota:** [estratégia].
- **Cuidados adicionais:** [não expor informações em logs, URL ou mensagens].

## 16. Critérios de aceitação específicos da interface

- [ ] Dado que [contexto], quando [ação], então [resultado visual].
- [ ] Durante o carregamento, a interface apresenta [comportamento].
- [ ] Quando não houver dados, a interface apresenta [mensagem/ação].
- [ ] Quando a API retornar erro, a interface [tratamento].
- [ ] A funcionalidade pode ser operada por teclado.

## 17. Evidências visuais

- **Protótipo no Figma:** [link]
- **Design System:** [link]
- **Captura da implementação:** [link ou imagem]
- **Storybook:** [link]

## 18. Rastreabilidade

- **Requisitos funcionais:** [RF-XXX]
- **Requisitos não funcionais:** [RNF-XXX]
- **Regras de negócio:** [RN-XXX]
- **Endpoints:** [API-XXX]
- **Componentes:** [COMP-XXX]
- **Casos de teste:** [CT-XXX]
- **Issue/épico:** [link]
- **Código-fonte:** [link]

## 19. Histórico de alterações

| Versão | Data | Responsável | Alteração |
|---|---|---|---|
| 1.0 | [AAAA-MM-DD] | [nome ou equipe] | Criação do documento |
