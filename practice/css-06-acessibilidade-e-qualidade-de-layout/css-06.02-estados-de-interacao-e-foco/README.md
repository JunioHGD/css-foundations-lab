# CSS-06.02 — Estados de Interação e Foco

Manter interfaces navegáveis por teclado e indicadores visuais claros (hover, foco, ativo).

## Fundamentos

- Estilos de hover e active (`:hover`, `:active`); realce de itens interativos.
- Indicador de foco (`:focus` ou `:focus-visible`): manter ou estilizar outline padrão para acessibilidade.
- Nunca remover completamente os estilos de foco (outline), pois isso prejudica usuários de teclado.
- Tamanho adequado de áreas clicáveis (paddings mínimos em botões ou links).

## Competências

Ao concluir esta unidade, devo conseguir:

- Assegurar que elementos interativos mostram estado visível quando focados via teclado.
- Diferenciar `:hover` (mouse) de `:focus` (teclado) e usar `:focus-visible` quando apropriado.
- Criar estilos evidentes (cores ou contornos) que indiquem foco, atendendo aos critérios de usabilidade.
- Evitar usar apenas cor para transmitir informação (ex.: “estilos importantes” usando cor + outro indicador).

## Prática

Os exercícios desta unidade aplicam os fundamentos estudados por meio de implementação, análise, diagnóstico e justificativa quando pertinentes.

[Ver exercícios →](./exercises/)

## Web Integration

Desenvolver um menu de navegação acessível que mostra outline nos links ao receber foco por Tab, e destacar o item atual via `:focus`.

[Ver Web Integration →](../../../web-integration/)

---

### Navegação

[← CSS-06.01 — Tipografia e Legibilidade](../css-06.01-tipografia-e-legibilidade/) ·
[↑ CSS-06 — Acessibilidade e Qualidade de Layout](../README.md) ·
[CSS-06.03 — Ocultamento e Ordens de Leitura →](../css-06.03-ocultamento-e-ordens-de-leitura/)
