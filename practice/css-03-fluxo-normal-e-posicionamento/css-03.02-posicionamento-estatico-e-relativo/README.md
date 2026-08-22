# CSS-03.02 — Posicionamento Estático e Relativo

Aprender os efeitos de `position: static` (padrão) e `position: relative` em elementos.

## Fundamentos

- Posição estática: o elemento permanece no fluxo normal (padrão).
- `position: relative`: desloca um elemento em relação à sua posição original sem removê-lo do fluxo (ex.: `left: 10px` desloca, mas espaço original é mantido).
- `top/right/bottom/left` em elementos relativos (movimentação a partir da posição inicial).
- Conceito básico de *containing block* para elementos relativamente posicionados (normalmente, o próprio elemento).
- Origem do sistema de coordenadas local para offsets.

## Competências

Ao concluir esta unidade, devo conseguir:

- Ajustar local rapidamente um elemento em relação à sua posição natural (ex.: criar um alinhamento fino).
- Prever como um `position: relative` afetará o layout (outro conteúdo não reposiciona totalmente).
- Usar deslocamentos sem quebrar o fluxo geral da página.

## Prática

Os exercícios desta unidade aplicam os fundamentos estudados por meio de implementação, análise, diagnóstico e justificativa quando pertinentes.

[Ver exercícios →](./exercises/)

## Web Integration

Posicionar um elemento de destaque levemente deslocado (por exemplo, um selo “New” sobre um banner) usando `position: relative` no elemento pai e `position: absolute` no selo (a ser visto em posicionamento absoluto). No contexto deste exercício, o foco será entender o deslocamento relativo antes de usar absoluto.

[Ver Web Integration →](../../../web-integration/)

---

### Navegação

[← CSS-03.01 — Fluxo normal (block vs inline) e display](../css-03.01-fluxo-normal-block-vs-inline-e-display/) ·
[↑ CSS-03 — Fluxo Normal e Posicionamento](../README.md) ·
[CSS-03.03 — Posicionamento Absoluto, Fixo, Sticky e Empilhamento →](../css-03.03-posicionamento-absoluto-fixo-sticky-e-empilhamento/)
