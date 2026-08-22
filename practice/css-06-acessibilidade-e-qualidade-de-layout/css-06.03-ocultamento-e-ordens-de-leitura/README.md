# CSS-06.03 — Ocultamento e Ordens de Leitura

Ocultar elementos de forma adequada sem prejudicar leitores de tela, e manter ordem lógica de conteúdo.

## Fundamentos

- `display: none` remove do fluxo e também da árvore de acessibilidade (conteúdo não é lido por leitores de tela).
- `visibility: hidden` esconde visualmente mas mantém espaço no layout; leitores de tela ainda verão o conteúdo (discutir quando usar cada um).
- Posicionamentos fora de tela (ex.: `position: absolute; left: -9999px`) para esconder conteúdo de layout mas mantê-lo disponível (ex.: texto alternativo).
- Leitura de conteúdo na ordem do DOM: mesmo que CSS reordene visualmente, manter estrutura HTML semântica (flex/grid não devem reordenar mentalmente o conteúdo sem necessidade).

## Competências

Ao concluir esta unidade, devo conseguir:

- Decidir como esconder conteúdo (por ex., menus móveis) sem quebrar acessibilidade.
- Garantir que a ordem de foco (tab order) segue o fluxo visual ou está clara.
- Justificar o uso de `display:none` vs outras técnicas para esconder conteúdo dinâmico.

## Prática

Os exercícios desta unidade aplicam os fundamentos estudados por meio de implementação, análise, diagnóstico e justificativa quando pertinentes.

[Ver exercícios →](./exercises/)

## Web Integration

Criar um menu “off-canvas” que aparece ao clicar num botão: usar `display:none` e depois `display:block` via CSS/JS, assegurando que o conteúdo escondido não confunda leitores de tela.

[Ver Web Integration →](../../../web-integration/)

---

### Navegação

[← CSS-06.02 — Estados de Interação e Foco](../css-06.02-estados-de-interacao-e-foco/) ·
[↑ CSS-06 — Acessibilidade e Qualidade de Layout](../README.md) ·
[Checkpoint CSS-06 →](../checkpoint/)
