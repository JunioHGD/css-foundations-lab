# CSS-05.02 — Media Queries e Breakpoints

Aprender a usar *Media Queries* para alterar estilos conforme condições (largura, orientação, resolução).

## Fundamentos

- Sintaxe das media queries (`@media (min-width: X)` etc.) e tipos de mídia (screen, print).
- Estratégia mobile-first: escrever CSS base para mobile e usar `min-width` para grandes telas.
- Definir breakpoints: identificar larguras em que o layout deve mudar.
- Adaptação de layout: reorganizar colunas em linhas, esconder/mostrar elementos, alterar tamanhos em diferentes faixas de tela.
- Conceito de *design adaptativo* vs *responsivo*.

## Competências

Ao concluir esta unidade, devo conseguir:

- Escrever regras CSS condicionais para diferentes tamanhos de viewport.
- Escolher breakpoints baseados no design (ex.: quando o conteúdo começa a ficar apertado).
- Testar no navegador usando ferramentas de desenvolvedor (alternância de dimensões).
- Justificar a escolha de um ponto de quebra específico com base na fluidez do conteúdo.

## Prática

Os exercícios desta unidade aplicam os fundamentos estudados por meio de implementação, análise, diagnóstico e justificativa quando pertinentes.

[Ver exercícios →](./exercises/)

## Web Integration

Implementar um design de site onde em telas estreitas (mobile) os itens ficam empilhados verticalmente, e em telas largas formam colunas horizontais. Exemplo: converter um menu de hambúrguer em barras horizontais via media query.

[Ver Web Integration →](../../../web-integration/)

---

### Navegação

[← CSS-05.01 — Layout Fluido e Unidades Relativas](../css-05.01-layout-fluido-e-unidades-relativas/) ·
[↑ CSS-05 — Responsividade e Adaptação](../README.md) ·
[Checkpoint CSS-05 →](../checkpoint/)
