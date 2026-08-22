# CSS-02.02 — Valores, Unidades e Tipografia

Aprender sobre os diferentes tipos de valores e unidades no CSS e como escolher unidades relativas ou absolutas para tamanhos e espaçamentos.

## Fundamentos

- Tipos de valores: numéricos, palavras-chave (ex.: `initial`, `inherit`) e funcionais (ex.: `calc()`).
- **Unidades absolutas:** `px`, `in`, `cm` (raramente usadas em web).
- **Unidades relativas:** `%`, `em`, `rem`, `vw`, `vh` etc.; entender referências de cálculo para cada uma.
- Importância de `em`/`rem` para escalabilidade de texto e layout (unidades relativas são mais acessíveis pois respeitam preferências do usuário).
- Uso de `%` para dimensões relativas ao elemento pai ou ao *containing block*.
- Unidades de cor (hexa, rgb(a), hsl(a)) e transparências básicas.

## Competências

Ao concluir esta unidade, devo conseguir:

- Definir tamanhos de fonte, largura e espaço com unidades adequadas para tornar o layout flexível.
- Usar `rem` para fontes baseadas no tamanho raiz e `em` para espaçamentos dependentes de fonte atual.
- Converter unidades quando necessário (por exemplo, de px para rem).
- Reconhecer situações onde `percentage` facilita layouts fluidos.

## Prática

Os exercícios desta unidade aplicam os fundamentos estudados por meio de implementação, análise, diagnóstico e justificativa quando pertinentes.

[Ver exercícios →](./exercises/)

## Web Integration

Implementar uma tipografia escalável: por exemplo, configurar `html { font-size: 100%; }` e usar `rem` para títulos, permitindo o ajuste proporcional se o usuário alterar o zoom/zoom da página.

[Ver Web Integration →](../../../web-integration/)

---

### Navegação

[← CSS-02.01 — Modelo de Caixa (Box Model)](../css-02.01-modelo-de-caixa-box-model/) ·
[↑ CSS-02 — Caixa e Dimensionamento](../README.md) ·
[CSS-02.03 — Dimensões, Largura/Altura e Overflow →](../css-02.03-dimensoes-largura-altura-e-overflow/)
