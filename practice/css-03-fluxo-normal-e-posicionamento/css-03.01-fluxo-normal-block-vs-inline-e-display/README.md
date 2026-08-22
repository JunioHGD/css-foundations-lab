# CSS-03.01 — Fluxo normal (block vs inline) e display

Entender como elementos de bloco e inline são posicionados em fluxo normal e como as propriedades `display` controlam isso.

## Fundamentos

- **Fluxo normal:** elementos em bloco (cada novo em linha) vs inline (no mesmo fluxo de linha).
- Propriedade `display`: valores básicos `block`, `inline`, `inline-block`, `none`, e noções de `flex`/`grid` como display (introdução).
- Colapso de margem entre elementos de bloco adjacentes.
- **Espaçamento branco (white-space)** e quebra automática de linha em texto inline.
- Conceito de *containing block* no contexto de elementos posicionados (ligado a fluxo).

## Competências

Ao concluir esta unidade, devo conseguir:

- Prever a posição inicial de elementos (por ex., duas `div` em sequência ficam empilhadas).
- Usar `display` para alterar o comportamento padrão (transformar bloco em inline-block, esconder elementos).
- Solucionar problemas de layout relacionados ao fluxo, como espaços indesejados entre elementos inline-block.
- Diferenciar `visibility: hidden` de `display: none` (impacto no fluxo).

## Prática

Os exercícios desta unidade aplicam os fundamentos estudados por meio de implementação, análise, diagnóstico e justificativa quando pertinentes.

[Ver exercícios →](./exercises/)

## Web Integration

Ajustar o layout de um cabeçalho com itens de menu: tornar elementos `li` em linha (`display:inline-block`) ou em bloco horizontal, garantindo que se comportem como desejado no fluxo.

[Ver Web Integration →](../../../web-integration/)

---

### Navegação

[↑ CSS-03 — Fluxo Normal e Posicionamento](../README.md) ·
[CSS-03.02 — Posicionamento Estático e Relativo →](../css-03.02-posicionamento-estatico-e-relativo/)
