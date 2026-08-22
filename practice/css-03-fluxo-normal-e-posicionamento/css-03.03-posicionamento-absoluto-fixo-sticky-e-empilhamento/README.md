# CSS-03.03 — Posicionamento Absoluto, Fixo, Sticky e Empilhamento

Aprender como remover elementos do fluxo e posicioná-los de forma independente, e como controlar a ordem de empilhamento (z-index).

## Fundamentos

- `position: absolute`: elemento sai do fluxo normal; posicionado em relação ao *containing block* (o ancestral posicionado mais próximo).
- `position: fixed`: elemento fixo em relação à viewport (sempre visível no mesmo lugar da tela).
- `position: sticky`: comportamento híbrido (posiciona como estático até certo ponto de scroll, depois se fixa).
- Como definir `top/right/bottom/left` nesses casos para posicionar o elemento precisamente.
- **Stacking context:** `z-index` define a ordem de sobreposição em contexto de empilhamento (possuem contexto elementos posicionados ou raiz); elementos com maior z-index aparecem na frente.

## Competências

Ao concluir esta unidade, devo conseguir:

- Colocar elementos em camadas sobrepostos de forma controlada (ex.: menus ou modais) usando `z-index`.
- Usar `position: absolute` para criar sobreposições, painéis popup ou ícones posicionados (ex.: texto sobre imagem).
- Entender como `fixed` garante barras fixas no topo/rodapé independente do scroll.
- Identificar *containing block* de um elemento absoluto (pai posicionado).

## Prática

Os exercícios desta unidade aplicam os fundamentos estudados por meio de implementação, análise, diagnóstico e justificativa quando pertinentes.

[Ver exercícios →](./exercises/)

## Web Integration

Construir um menu fixo no topo da página (`fixed`) ou uma caixa de diálogo posicionada (`absolute`) sobre o conteúdo; por exemplo, um modal ou tooltip que requer posicionamento fora do fluxo normal.

[Ver Web Integration →](../../../web-integration/)

---

### Navegação

[← CSS-03.02 — Posicionamento Estático e Relativo](../css-03.02-posicionamento-estatico-e-relativo/) ·
[↑ CSS-03 — Fluxo Normal e Posicionamento](../README.md) ·
[CSS-03.04 — Floats e Layout Legado (conteúdo opcional) →](../css-03.04-floats-e-layout-legado-conteudo-opcional/)
