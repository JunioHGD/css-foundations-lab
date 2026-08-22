# CSS-05.01 — Layout Fluido e Unidades Relativas

Dominar técnicas para fazer componentes dimensionais fluírem com o tamanho da tela ou contêiner.

## Fundamentos

- Layout líquido: definir larguras com `%`, `vw`, `vh` para preencher contêineres fluentes.
- Uso de `max-width` para limitar crescimento (ex.: evitar que texto fique muito largo).
- Imagens e mídias fluídas: `img { max-width: 100%; height: auto; }` para redimensionar imagens dentro do contêiner.
- Unidades de viewport (`vw`, `vh`) para font-size ou larguras relativas ao tamanho da janela.
- Conceito de tipografia responsiva: `clamp()`, tamanhos base em `rem` e espaçamento proporcional.

## Competências

Ao concluir esta unidade, devo conseguir:

- Criar colunas que se redimensionam (porcentagens em `width`).
- Garantir que mídias (imagens, vídeos) nunca ultrapassem seus contêineres.
- Evitar layout fixo em pixels, preferindo unidades flexíveis.
- Antecipar como elementos redimensionam quando a janela muda de tamanho.

## Prática

Os exercícios desta unidade aplicam os fundamentos estudados por meio de implementação, análise, diagnóstico e justificativa quando pertinentes.

[Ver exercícios →](./exercises/)

## Web Integration

Construir um grid responsivo onde as colunas crescem/encolhem conforme o navegador; ajustar imagens e textos para que redimensionem sem distorção, mantendo proporção e legibilidade.

[Ver Web Integration →](../../../web-integration/)

---

### Navegação

[↑ CSS-05 — Responsividade e Adaptação](../README.md) ·
[CSS-05.02 — Media Queries e Breakpoints →](../css-05.02-media-queries-e-breakpoints/)
