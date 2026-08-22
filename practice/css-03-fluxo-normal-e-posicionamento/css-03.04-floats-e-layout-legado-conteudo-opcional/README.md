# CSS-03.04 — Floats e Layout Legado (conteúdo opcional)

Compreender o uso original da propriedade `float` e seu impacto no fluxo (técnicas legadas de layout).

## Fundamentos

- `float: left/right`: tira o elemento do fluxo de texto normal e faz o texto fluir ao redor dele (como no layout de imagem com texto contornando).
- Problemas de *clear* (limpeza): quando elementos subsequentes podem fluir para o lado do *float*, uso de `clear: both` para quebrar o fluxo.
- Uso histórico de floats para criar layouts de colunas antes do flex/grid (técnica legada).

## Competências

Ao concluir esta unidade, devo conseguir:

- Aplicar float em elementos para fazer texto contornar (como imagens em parágrafos).
- Resolver colapsos de altura em contêineres que têm apenas filhos flutuantes (ex.: clearfix).
- Reconhecer quando não usar float em layouts modernos (preferir flex/grid para colunas).

## Prática

Os exercícios desta unidade aplicam os fundamentos estudados por meio de implementação, análise, diagnóstico e justificativa quando pertinentes.

[Ver exercícios →](./exercises/)

## Web Integration

Flutuar uma imagem à esquerda de um parágrafo, garantindo que o texto se ajuste corretamente (float). Em um contexto de integração, adicionar clareza de funcionamento comparando com Flexbox para colunas como alternativa.

[Ver Web Integration →](../../../web-integration/)

---

### Navegação

[← CSS-03.03 — Posicionamento Absoluto, Fixo, Sticky e Empilhamento](../css-03.03-posicionamento-absoluto-fixo-sticky-e-empilhamento/) ·
[↑ CSS-03 — Fluxo Normal e Posicionamento](../README.md) ·
[Checkpoint CSS-03 →](../checkpoint/)
