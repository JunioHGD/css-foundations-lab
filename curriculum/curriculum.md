# CSS Foundations Lab — Currículo

## Objetivo
Dominar os fundamentos de CSS necessários para construir, compreender e manter interfaces web responsivas e acessíveis. O Lab desenvolve competência funcional de frontend para apoiar projetos web e a futura atuação em backend.

## Método de estudo
1. Estudar sequencialmente os tópicos de cada módulo, realizando pequenas experimentações quando necessário.
2. Concluir **um exercício integrador por módulo**, aplicando os tópicos relacionados.
3. Conferir critérios de conclusão, depurar problemas e registrar aprendizados relevantes.

**Concluído significa:** conseguir explicar o mecanismo, utilizá-lo com autonomia e corrigir erros comuns. Não é necessário explorar todos os recursos avançados da linguagem para avançar.

**Limite do Lab:** CSS trabalha apresentação, layout, estados visuais e adaptação. Os exercícios usam HTML como base, sem exigir lógica JavaScript não estudada; interações por JavaScript são complementares. Acessibilidade visual e responsividade devem ser consideradas progressivamente, não apenas nos módulos finais.

## Percurso

| Módulo | Conteúdos | Tópicos | Exercício integrador |
| --- | --- | :---: | --- |
| [CSS-01 — Seletores, Cascata e Herança](../modules/css-01-seletores-especificidade-e-cascata/) | Compreender como as regras de CSS atingem elementos e como o navegador determina os estilos aplicados | 2 | Diagnóstico de estilos |
| [CSS-02 — Modelo de Caixa e Estilização](../modules/css-02-caixa-e-dimensionamento/) | Controlar dimensões, espaçamentos e aparência sem provocar cortes ou transbordamentos desnecessários | 3 | Painel de cartões ajustáveis |
| [CSS-03 — Fluxo Normal e Posicionamento](../modules/css-03-fluxo-normal-e-posicionamento/) | Entender a disposição padrão dos elementos e aplicar posicionamento quando realmente necessário | 3 | Interface com elementos posicionados |
| [CSS-04 — Layouts com Flexbox e Grid](../modules/css-04-layout-com-flexbox-e-grid/) | Construir layouts modernos escolhendo corretamente entre distribuição unidimensional e bidimensional | 2 | Dashboard em Grid e Flexbox |
| [CSS-05 — Responsividade e Adaptação](../modules/css-05-responsividade-e-adaptacao/) | Fazer interfaces funcionarem em larguras e preferências de visualização diferentes | 2 | Página responsiva de serviços |
| [CSS-06 — Acessibilidade Visual e Qualidade](../modules/css-06-acessibilidade-e-qualidade-de-layout/) | Garantir que estilos preservem legibilidade, foco, sequência de leitura e uso com diferentes preferências | 3 | Revisão de acessibilidade de uma interface |

---

## CSS-01 — Seletores, Cascata e Herança

**Objetivo:** Compreender como as regras de CSS atingem elementos e como o navegador determina os estilos aplicados.

**Pré-requisito:** HTML básico e estrutura de páginas

### CSS-01.01 — Sintaxe e seletores

- Regra CSS: seletor, declaração, propriedade, valor, comentários e folha de estilos externa.
- Seletores de tipo, classe, ID e atributo; combinadores de descendência e filho direto.
- Pseudoclasses de estado, como `:hover`, `:focus-visible` e `:disabled`, e pseudoelementos básicos (`::before`, `::after`).

### CSS-01.02 — Cascata, especificidade e herança

- Prioridade entre declarações: origem, importância (`!important`), camadas de cascata, especificidade e ordem de aparição, conforme aplicável. Usar `!important` com critério, não como correção automática.
- Propriedades herdadas e não herdadas; valores `inherit`, `initial` e `unset`; estilos padrão do navegador.
- Depuração no DevTools (painéis Styles/Computed), organização de seletores e valores personalizados (`--variavel`, `var()`) para reduzir repetição de cores e espaços.

### Competências esperadas

- Explicar por que uma declaração foi aplicada ou substituída.
- Escrever seletores previsíveis, evitando especificidade desnecessária.
- Identificar conflitos e corrigi-los pelo DevTools, sem depender de `!important`.

### Exercício integrador

**Diagnóstico de estilos** — Corrigir uma interface com regras conflitantes, estados visuais inconsistentes e valores repetidos.

**Critérios de conclusão**

- Identificar as regras vencedoras e justificar ao menos três correções.
- Utilizar classes e variáveis CSS de maneira coerente.
- Preservar estilos de foco e estados interativos.

[Abrir módulo no repositório](../modules/css-01-seletores-especificidade-e-cascata/)

---

## CSS-02 — Modelo de Caixa e Estilização

**Objetivo:** Controlar dimensões, espaçamentos e aparência sem provocar cortes ou transbordamentos desnecessários.

**Pré-requisito:** módulo CSS-01

### CSS-02.01 — Modelo de caixa

- Conteúdo, `padding`, `border` e `margin`; diferenças entre `content-box` e `border-box`, incluindo uso global criterioso de `box-sizing: border-box`.
- Cálculo do espaço ocupado e colapso de margens verticais, em situações aplicáveis.

### CSS-02.02 — Valores, unidades e aparência

- Unidades `px`, `%`, `em`, `rem`, `vw`, `vh` e noções de `calc()`; referência utilizada por cada unidade.
- Cor, fundo, transparência, bordas, arredondamento, famílias de fontes, peso, tamanho e altura de linha; distinguir cor de texto de cor de fundo e manter contraste adequado.
- Escolha de unidades adequadas ao conteúdo, respeitando zoom e preferências de tamanho do usuário.

### CSS-02.03 — Dimensionamento e overflow

- `width`, `height`, `min-*`, `max-*`, `auto` e dimensionamento intrínseco.
- `overflow`, imagens que se ajustam ao contêiner, `aspect-ratio` e `object-fit` nos casos apropriados.
- Diagnóstico de transbordamento horizontal, palavras/URLs longas e dimensões excessivamente rígidas; aplicar `overflow-wrap` e limites de largura sem esconder conteúdo importante.

### Competências esperadas

- Calcular e ajustar corretamente tamanho e espaçamento dos elementos.
- Estilizar tipografia, fundos e bordas de forma consistente.
- Corrigir overflow sem ocultar conteúdo importante.

### Exercício integrador

**Painel de cartões ajustáveis** — Construir uma composição de cartões com espaçamento, tipografia, dimensões e conteúdos de tamanhos diferentes.

**Critérios de conclusão**

- Demonstrar domínio do box model e das unidades escolhidas.
- Evitar transbordamento e perda de conteúdo em larguras menores.
- Manter apresentação visual legível e consistente.

[Abrir módulo no repositório](../modules/css-02-caixa-e-dimensionamento/)

---

## CSS-03 — Fluxo Normal e Posicionamento

**Objetivo:** Entender a disposição padrão dos elementos e aplicar posicionamento quando realmente necessário.

**Pré-requisito:** módulo CSS-02

### CSS-03.01 — Fluxo normal e display

- Diferença entre comportamento de caixas `block`, `inline` e `inline-block`.
- Valores de `display` e efeitos no fluxo; `display: none` e `visibility: hidden`.
- Fluxo do texto, quebras de linha e efeitos de espaçamento.

### CSS-03.02 — Posicionamento relativo e absoluto

- `position: static`, `relative` e `absolute`; offsets e noção de *containing block*.
- Quando elementos permanecem no fluxo e quando deixam de ocupar espaço nele.
- Sobreposições localizadas, como indicadores em cartões, evitando posicionar layouts inteiros com offsets.

### CSS-03.03 — Posicionamento fixo, sticky e empilhamento

- `position: fixed` e `sticky`, limites do contêiner de rolagem e efeitos na experiência de navegação.
- `z-index` e contexto de empilhamento; causas comuns de elementos sobrepostos incorretamente.
- Como inspecionar problemas de empilhamento e manter conteúdo acessível.

### Competências esperadas

- Prever a posição de elementos no fluxo normal.
- Escolher entre fluxo, Flexbox/Grid e posicionamento para o problema certo.
- Controlar sobreposições e camadas sem quebrar a leitura do documento.

### Exercício integrador

**Interface com elementos posicionados** — Montar uma página com conteúdo em fluxo normal, selo sobre um cartão e cabeçalho ou região sticky.

**Critérios de conclusão**

- Usar cada tipo de posicionamento com finalidade justificável.
- Evitar sobreposição que bloqueie controles ou conteúdo.
- Explicar o contexto de referência dos elementos posicionados.

**Consulta sob demanda:** `float` e `clear` para leitura de código legado ou texto contornando imagens; não são pré-requisitos para layouts modernos.

[Abrir módulo no repositório](../modules/css-03-fluxo-normal-e-posicionamento/)

---

## CSS-04 — Layouts com Flexbox e Grid

**Objetivo:** Construir layouts modernos escolhendo corretamente entre distribuição unidimensional e bidimensional.

**Pré-requisito:** módulo CSS-03

### CSS-04.01 — Flexbox

- Contêiner e itens flex; eixo principal e transversal; `justify-content`, `align-items` e `gap`.
- `flex-direction`, `flex-wrap`, `flex-grow`, `flex-shrink`, `flex-basis` e tamanhos mínimos automáticos dos itens; corrigir overflow quando necessário com `min-width: 0`.
- Padrões comuns: navegação, cartões em linha, alinhamento de botões e componentes.

### CSS-04.02 — CSS Grid

- Definição de linhas e colunas com `grid-template-*`, unidades `fr` e `gap`.
- Posicionamento e dimensionamento com `repeat()`, `minmax()`, `auto-fit` e `auto-fill`; entender como conteúdos grandes influenciam o mínimo das trilhas.
- Diferenças práticas entre Grid e Flexbox; composição de regiões e grades de cartões.

### Competências esperadas

- Escolher Flexbox ou Grid em função das dimensões do layout.
- Controlar alinhamento, distribuição e preenchimento disponível.
- Criar uma estrutura de página legível sem truques de posicionamento absoluto.

### Exercício integrador

**Dashboard em Grid e Flexbox** — Construir um painel simples de informações com cabeçalho, navegação, cartões e área principal.

**Critérios de conclusão**

- Aplicar Grid ao arranjo principal e Flexbox a componentes internos.
- Manter alinhamentos previsíveis quando o conteúdo muda.
- Justificar a escolha de cada mecanismo de layout.

[Abrir módulo no repositório](../modules/css-04-layout-com-flexbox-e-grid/)

---

## CSS-05 — Responsividade e Adaptação

**Objetivo:** Fazer interfaces funcionarem em larguras e preferências de visualização diferentes.

**Pré-requisito:** módulo CSS-04

### CSS-05.01 — Layouts fluidos

- Abordagem mobile-first, contêineres fluidos e limites com `min-width`/`max-width`; verificar a presença do metadado HTML `viewport` para páginas móveis.
- Unidades relativas aplicadas ao layout; `min()`, `max()` e `clamp()` em situações úteis.
- Imagens, grades e textos que se adaptam sem depender de dimensões fixas.

### CSS-05.02 — Media queries e breakpoints

- Sintaxe de `@media`, consultas de largura e preferência do usuário quando relevantes.
- Definição de pontos de quebra pelo comportamento do conteúdo, não por modelos fixos de aparelhos.
- Teste em larguras pequenas, intermediárias e grandes usando DevTools, inclusive zoom e aumento de fonte; verificar scroll horizontal e controles fora da tela.

### Competências esperadas

- Construir layouts utilizáveis no celular e desktop.
- Escolher breakpoints segundo o conteúdo e não apenas por convenção.
- Inspecionar e corrigir problemas de adaptação entre diferentes larguras.

### Exercício integrador

**Página responsiva de serviços** — Desenvolver uma página com lista de serviços e componentes reorganizados conforme a largura disponível.

**Critérios de conclusão**

- Testar larguras pequenas, intermediárias e grandes.
- Manter boa legibilidade e navegação em diferentes tamanhos.
- Evitar overflow horizontal e controles difíceis de acionar.

[Abrir módulo no repositório](../modules/css-05-responsividade-e-adaptacao/)

---

## CSS-06 — Acessibilidade Visual e Qualidade

**Objetivo:** Garantir que estilos preservem legibilidade, foco, sequência de leitura e uso com diferentes preferências.

**Pré-requisito:** módulo CSS-05

### CSS-06.01 — Tipografia e legibilidade

- Tamanho e espaçamento de texto, comprimento de linha, altura de linha e alinhamento.
- Contraste de texto e elementos informativos; estados não indicados apenas por cor.
- Zoom, aumento de texto e impacto de fontes rígidas sobre a leitura.

### CSS-06.02 — Estados interativos e foco

- Estilos visíveis de `:focus-visible`, `:hover`, `:active`, `:disabled` e estados de formulários; não comunicar erro/sucesso exclusivamente pela cor.
- Distinção entre interação por mouse, teclado e toque; não remover foco sem alternativa.
- Transições curtas quando acrescentarem feedback e respeito a `prefers-reduced-motion` quando houver movimento; animações complexas não são pré-requisito.

### CSS-06.03 — Visibilidade e ordem de leitura

- Diferenças entre `display: none`, `visibility: hidden` e transparência em relação a layout, interação e acessibilidade.
- Ordem visual com Flexbox/Grid versus ordem do DOM e navegação por teclado.
- Limites da responsabilidade do CSS: não inserir conteúdo semântico indispensável apenas por pseudoelementos; HTML fornece significado e JavaScript fornece comportamento.

### Competências esperadas

- Encontrar e corrigir problemas de contraste, foco e legibilidade.
- Preservar ordem de leitura e navegação coerentes.
- Escolher estratégias de ocultação e movimento sem prejudicar a acessibilidade.

### Exercício integrador

**Revisão de acessibilidade de uma interface** — Receber uma página com problemas de legibilidade, foco, ordem visual e adaptação e corrigi-los.

**Critérios de conclusão**

- Demonstrar foco visível e contraste adequado.
- Verificar zoom, teclado e diferentes tamanhos de tela.
- Explicar os limites de uma solução feita apenas em CSS.

[Abrir módulo no repositório](../modules/css-06-acessibilidade-e-qualidade-de-layout/)

---

## Verificação prática ao concluir o Lab

- Testar interface em celular e desktop, larguras intermediárias, zoom e teclado; confirmar que informação importante não foi cortada.
- Inspecionar cascata, dimensões, alinhamentos e overflow pelo DevTools antes de adicionar regras corretivas.
- Validar estados de foco, legibilidade e contraste. Ajustes responsivos e acessíveis fazem parte da qualidade da solução, não são recursos extras.

**Próximas tecnologias:** JavaScript acrescentará comportamento e estado ao HTML e ao CSS; não é necessário aprendê-lo para demonstrar as competências básicas deste Lab.

## Referências para consulta

- [MDN — Fundamentos de CSS](https://developer.mozilla.org/en-US/curriculum/core/css-fundamentals/)
- [MDN — Layout CSS](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/CSS_layout)
- [MDN — Acessibilidade com CSS e JavaScript](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Accessibility/CSS_and_JavaScript)
