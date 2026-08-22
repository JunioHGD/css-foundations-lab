# CSS-02.03 — Dimensões, Largura/Altura e Overflow

Controlar explicitamente as dimensões (width, height, min/max) de elementos e lidar com conteúdo que extrapola essas dimensões (overflow).

## Fundamentos

- Propriedades `width`, `height`, `min-width`, `max-width`, `min-height`, `max-height` e como elas afetam o tamanho de boxes.
- Diferença entre valores fixos (px) e fluidos (% ou `auto`) nas dimensões.
- Comportamento do overflow: `overflow: visible/hidden/scroll/auto`. O que acontece quando o conteúdo não cabe (scrollbars, corte).
- Uso de `max-width: 100%` em imagens para evitar ultrapassar o contêiner (funda­mental para responsividade).

## Competências

Ao concluir esta unidade, devo conseguir:

- Definir limites de tamanho (ex.: páginas centradas com `max-width` para legibilidade).
- Prever quando o conteúdo causará overflow e escolher estratégia (cortar, rolagem ou ajuste de layout).
- Aplicar porcentagens de forma que elementos se ajustem ao pai (ex.: colunas fluidas).
- Utilizar `box-sizing` (de 02.01) em conjunto para garantir que `width` inclua padding/borda conforme esperado.

## Prática

Os exercícios desta unidade aplicam os fundamentos estudados por meio de implementação, análise, diagnóstico e justificativa quando pertinentes.

[Ver exercícios →](./exercises/)

## Web Integration

Resolver um caso em que um painel de conteúdo está excedendo seu contêiner. Por exemplo, exibir barras de rolagem apenas quando necessário usando `overflow`, ou fazer imagens responsivas com `max-width: 100%`.

[Ver Web Integration →](../../../web-integration/)

---

### Navegação

[← CSS-02.02 — Valores, Unidades e Tipografia](../css-02.02-valores-unidades-e-tipografia/) ·
[↑ CSS-02 — Caixa e Dimensionamento](../README.md) ·
[Checkpoint CSS-02 →](../checkpoint/)
