---
name: design-skills
description: Conhecimento de UX e design de produto em uma skill só, com 10 áreas. Crítica e avaliação heurística (Nielsen, leis de UX), auditoria de acessibilidade WCAG 2.2, design systems (tokens, componentes, governança), design de interação (microinterações, estados, motion, prevenção de erros), UX writing (microcopy, erros, voz e tom), pesquisa de UX (entrevistas, testes de usabilidade, síntese), estratégia de UX (JTBD, análise competitiva, métricas HEART), mapas de jornada e service blueprints, design ops (sprints, handoff, design QA) e refinamento visual de telas, dashboards e relatórios. Use ao desenhar, revisar, criticar, especificar ou documentar qualquer interface, fluxo, componente ou texto de interface, e ao planejar pesquisa ou estratégia de produto. Aciona com "critica essa tela", "revisa a usabilidade", "está acessível?", "especifica esse componente", "escreve a mensagem de erro", "roteiro de entrevista", "mapa de jornada", "handoff para dev", "deixa esse layout mais profissional", em português, inglês ou espanhol.
---

# Design Skills

Esta skill junta as 10 skills de [cuellarfr/design-skills](https://github.com/cuellarfr/design-skills). Cada área tem um guia próprio em `areas/<área>/GUIDE.md`, que funciona sozinho, e pastas de apoio carregadas só quando necessário:

- `references/`: aprofundamento de um tema
- `templates/`: modelos de entregáveis para preencher
- `examples/`: exemplos completos de ponta a ponta

**Caminhos:** dentro de cada `GUIDE.md`, os caminhos como `references/x.md` são relativos à pasta da área. Por exemplo, `references/wcag-checklist.md` no guia de acessibilidade corresponde a `areas/accessibility-audit/references/wcag-checklist.md`.

## Como usar

1. Identifique a área (ou áreas) pela tabela abaixo.
2. Leia o `GUIDE.md` da área **antes** de responder. Não responda de memória quando o guia cobre o assunto.
3. Abra `references/`, `templates/` ou `examples/` apenas quando o guia indicar ou a tarefa pedir profundidade.
4. Fundamente cada recomendação em um princípio, heurística ou método citado no guia. Não use preferência pessoal como justificativa.
5. Responda no idioma do usuário. O material de referência está em inglês: traduza termos quando fizer sentido e mantenha o nome original de frameworks e métodos (por exemplo, "Jobs to Be Done" ou "Service Blueprint").

## Roteamento por área

| Pedido | Área | Guia |
|---|---|---|
| Avaliar, criticar ou revisar uma tela ou fluxo; avaliação heurística; escolher um padrão de interação; avaliar arquitetura de informação | Crítica de design | `areas/design-critique/GUIDE.md` |
| Checar acessibilidade, WCAG, contraste, navegação por teclado, leitor de tela, HTML semântico | Acessibilidade | `areas/accessibility-audit/GUIDE.md` |
| Tokens, especificação de componentes, nomenclatura, inventário de interface, governança, maturidade do sistema | Design systems | `areas/design-systems/GUIDE.md` |
| Microinterações, estados de componente, animação, gestos, loading, undo, prevenção e recuperação de erros | Design de interação | `areas/interaction-design/GUIDE.md` |
| Textos de botões, labels, mensagens de erro e sucesso, empty states, onboarding, notificações, voz e tom | UX writing | `areas/ux-writing/GUIDE.md` |
| Plano de pesquisa, roteiro de entrevista, teste de usabilidade, recrutamento, síntese, personas | Pesquisa de UX | `areas/ux-research/GUIDE.md` |
| Resultados de negócio, JTBD, análise competitiva, proposta de valor, métricas (HEART, North Star), Opportunity Solution Tree | Estratégia de UX | `areas/ux-strategy/GUIDE.md` |
| Mapa de jornada, service blueprint, mapa de empatia, experience map, workshop de alinhamento, diagramas de fluxo | Mapeamento de jornada | `areas/journey-mapping/GUIDE.md` |
| Design sprint, handoff para desenvolvimento, rituais de time, documentação, design QA | Design ops | `areas/design-ops/GUIDE.md` |
| Levar uma saída visual (tela, dashboard, relatório, HTML, apresentação, gráfico) de funcional a refinada: grid, tipografia, cor, espaçamento, visualização de dados | Refinamento visual | `areas/design-elevation/GUIDE.md` |

Quando o pedido é ambíguo, prefira a área mais próxima do entregável solicitado. Por exemplo, "melhora essa tela" com foco em problemas de uso vai para crítica de design; com foco em aparência, vai para refinamento visual.

## Pedidos que envolvem várias áreas

Carregue apenas os guias necessários, na ordem em que o trabalho acontece:

- **Revisão completa de uma tela:** crítica de design, depois acessibilidade, depois UX writing (textos da tela).
- **Especificar um componente novo:** design systems (especificação e tokens), depois design de interação (inventário de estados), depois acessibilidade (requisitos do componente).
- **Novo fluxo ou funcionalidade:** estratégia de UX (resultado esperado), depois mapeamento de jornada (situação atual e futura), depois design de interação (comportamento).
- **Validar com usuários:** pesquisa de UX (plano e roteiro), depois crítica de design (hipóteses a testar a partir dos problemas encontrados).
- **Entregar para desenvolvimento:** design ops (checklist de handoff e design QA), depois design systems (tokens e nomes dos componentes).

## Observações por área

- **Refinamento visual:** usa os tokens do Tailwind CSS como referência e traz tabelas de design systems corporativos (Carbon, Polaris, Spectrum, Lightning, Modus) em `references/`. Quando o projeto já tem um design system próprio, os tokens do projeto prevalecem; use o guia pelo método (grid, hierarquia, interrogação das escolhas), não para substituir a identidade existente. O guia pede execução silenciosa, ou seja, aplicar o processo sem narrá-lo, a menos que o usuário peça a explicação.
- **Acessibilidade:** `templates/accessibility-rules-file.md` é um modelo de regras para arquivos de instrução de agentes (CLAUDE.md, .cursorrules). Use-o quando o objetivo for prevenir problemas em UI gerada, não só auditar.
- **UX writing:** `docs/figma-integration.md` cobre o trabalho de textos direto no Figma.

## Fonte e licença

Conteúdo copiado sem alterações de [cuellarfr/design-skills](https://github.com/cuellarfr/design-skills) (site: https://cuellarfr.github.io/design-skills/), commit `b41750a` (23/08/2026). Os `SKILL.md` originais viraram `areas/<área>/GUIDE.md`, e só o cabeçalho YAML foi removido. Licença MIT, Copyright (c) 2026 Carlos C., conforme `LICENSE`.

Para atualizar, clone o repositório de origem e copie `skills/<área>/*` para `areas/<área>/`, renomeando `SKILL.md` para `GUIDE.md` e removendo o cabeçalho YAML.
