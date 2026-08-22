# CSS-01.02 — Cascata, Especificidade e Herança

Compreender como o CSS **resolve conflitos** entre regras, determinar a especificidade de seletores e o papel da herança e da ordem das declarações.

## Fundamentos

- **Cascata:** origem e ordem das regras (user agent, user, author) e o papel de `!important`.
- **Especificidade:** algoritmo que define peso de seletores (id > classe > elemento).
- **Herança:** propriedades que são herdadas (ex.: `color`, `font-family`) versus propriedades que não o são (ex.: `width`). Valores iniciais padrões.
- Como depurar conflitos comuns: declarar a mesma propriedade em regras diferentes, entender qual prevalece.

## Competências

Ao concluir esta unidade, devo conseguir:

- Prever qual regra será aplicada quando múltiplas regras afetem o mesmo elemento/propriedade.
- Diagnosticar por que um estilo esperado não aparece (ex.: seletor errado, menor especificidade, ordem incorreta).
- Justificar decisões de estilo explicando origem, especificidade e herança das regras.
- Evitar hackeações simples, preferindo reorganizar CSS ou aumentar especificidade conscientemente.

## Prática

Os exercícios desta unidade aplicam os fundamentos estudados por meio de implementação, análise, diagnóstico e justificativa quando pertinentes.

[Ver exercícios →](./exercises/)

## Web Integration

Resolver um problema de cascata em que diferentes arquivos CSS (ou estilos inline) definem a mesma propriedade. Ex.: um script JS alterna classes e o aluno explica por que o estilo resultante veio de uma regra específica (especificidade e ordem).

[Ver Web Integration →](../../../web-integration/)

---

### Navegação

[← CSS-01.01 — Seletores CSS](../css-01.01-seletores-css/) ·
[↑ CSS-01 — Seletores, Especificidade e Cascata](../README.md) ·
[Checkpoint CSS-01 →](../checkpoint/)
