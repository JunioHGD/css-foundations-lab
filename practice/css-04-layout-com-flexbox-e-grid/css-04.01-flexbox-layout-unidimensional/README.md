# CSS-04.01 — Flexbox (Layout Unidimensional)

Entender o **modelo flexbox**, dispondo itens em um único eixo (linha ou coluna) de maneira flexível.

## Fundamentos

- Contêiner flexível (`display: flex` ou `inline-flex`) e flex items (filhos diretos).
- Eixos do flexbox: eixo principal (main axis) e cruzado (cross axis).
- Propriedades do contêiner: `flex-direction` (row/column), `flex-wrap` (embrulhar ou não), `justify-content` (distribuição no eixo principal), `align-items` (alinhamento no eixo cruzado).
- Propriedades dos itens: `flex-grow`, `flex-shrink`, `flex-basis` (dimensões flexíveis), alinhamento individual (`align-self`).
- Ordenação de itens (`order`) e impactos.

## Competências

Ao concluir esta unidade, devo conseguir:

- Criar colunas ou filas iguais facilmente (por exemplo, 3 cards lado a lado que se expandem igualmente).
- Centralizar itens no eixo principal ou cruzado sem ajustes de margem.
- Resolver excesso de conteúdo usando `flex-wrap`.
- Comparar cenários: **quando usar flexbox** em vez de grid ou fluxo normal (situações 1D, filas flexíveis).

## Prática

Os exercícios desta unidade aplicam os fundamentos estudados por meio de implementação, análise, diagnóstico e justificativa quando pertinentes.

[Ver exercícios →](./exercises/)

## Web Integration

Implementar um layout de “cards” onde cada linha deve conter um número variável de itens que se ajustam ao espaço. Por exemplo, um cabeçalho com itens de navegação distribuidos uniformemente no eixo principal, ou uma galeria responsiva de cartões usando `flex`.

[Ver Web Integration →](../../../web-integration/)

---

### Navegação

[↑ CSS-04 — Layout com Flexbox e Grid](../README.md) ·
[CSS-04.02 — CSS Grid (Layout Bidimensional) →](../css-04.02-css-grid-layout-bidimensional/)
