# CSS-02.01 — Modelo de Caixa (Box Model)

Entender que cada elemento é uma caixa composta por conteúdo, padding, borda e margem, e como ajustar esses valores.

## Fundamentos

- Estrutura da caixa: conteúdo, `padding`, `border`, `margin`.
- Modelo de caixa padrão (`content-box`) vs `box-sizing: border-box`.
- Cálculo de largura/altura total de um elemento (por exemplo, `width` + padding + borda em *content-box*).
- Colapso de margens verticais (quando margens de elementos em bloco se fundem).
- Conceito de *containing block* para elementos relativos (relevante em posicionamento futuro).

## Competências

Ao concluir esta unidade, devo conseguir:

- Calcular manualmente a largura/altura ocupada por um elemento, considerando padding e bordas.
- Usar `box-sizing` para alterar esse comportamento conforme necessidade.
- Ajustar margens e espaçamentos para manter alinhamentos previsíveis.
- Prever efeitos do colapso de margens em elementos sequenciais.

## Prática

Os exercícios desta unidade aplicam os fundamentos estudados por meio de implementação, análise, diagnóstico e justificativa quando pertinentes.

[Ver exercícios →](./exercises/)

## Web Integration

Criar um “cartão” visual (card) onde se ajusta padding e margem para alinhar texto e imagem interna. Por exemplo, definir `box-sizing:border-box` para que o `width` defina o tamanho total do card, evitando overflow.

[Ver Web Integration →](../../../web-integration/)

---

### Navegação

[↑ CSS-02 — Caixa e Dimensionamento](../README.md) ·
[CSS-02.02 — Valores, Unidades e Tipografia →](../css-02.02-valores-unidades-e-tipografia/)
