# CSS Foundations Lab — Currículo Canônico

## Escopo

O **CSS Foundations Lab** desenvolve compreensão dos mecanismos essenciais que controlam apresentação e layout na Web. O foco está em seleção, cascata, especificidade, herança, modelo de caixa, fluxo, posicionamento, Flexbox, Grid, responsividade e acessibilidade visual, com ênfase em prever, explicar e diagnosticar comportamentos.

## Mapa curricular

| ID | Bloco |
|:---:|---|
| `CSS-01` | [Seletores, Especificidade e Cascata](../practice/css-01-seletores-especificidade-e-cascata/) |
| `CSS-02` | [Caixa e Dimensionamento](../practice/css-02-caixa-e-dimensionamento/) |
| `CSS-03` | [Fluxo Normal e Posicionamento](../practice/css-03-fluxo-normal-e-posicionamento/) |
| `CSS-04` | [Layout com Flexbox e Grid](../practice/css-04-layout-com-flexbox-e-grid/) |
| `CSS-05` | [Responsividade e Adaptação](../practice/css-05-responsividade-e-adaptacao/) |
| `CSS-06` | [Acessibilidade e Qualidade de Layout](../practice/css-06-acessibilidade-e-qualidade-de-layout/) |

---

# CSS-01 — Seletores, Especificidade e Cascata

## Objetivo

Desenvolver a capacidade de **aplicar estilos de forma previsível** sabendo como selecionar elementos corretamente e resolver conflitos entre regras. Ao final, o aluno deve entender de onde vêm os valores dos estilos e por que determinada regra CSS prevalece sobre outra.

## Unidades

### CSS-01.01 — Seletores CSS

**Objetivo**

Aprender a **escolher e escrever seletores** que atingem corretamente os elementos-alvo no HTML.

**Fundamentos**

- Sintaxe de regra CSS (seletor { propriedade: valor; }) e relacioná-la ao DOM.
- Seletores de tipo, classe, id, atributo, descendente, filho e irmãos.
- Pseudoclasses essenciais (`:hover`, `:focus`, `:active`, `:visited`) e pseudoelementos básicos (`::before`, `::after`) para estilização reativa.

**Competências**

- Selecionar elementos usando diferentes combinadores.
- Associar estilos a interações básicas (hover, foco) por pseudoclasses.
- Prever quais elementos serão afetados por determinado seletor.
- Evitar seletores excessivamente genéricos ou específicos demais.

**Dependências**

nenhuma (pré-requisito básico de HTML).

**Web Integration**

Estilizar um menu de navegação que muda aparência no `:hover` ou no estado de foco via teclado. Por exemplo, JS pode adicionar/remover classes a elementos de menu; o aluno deve aplicar seletores adequados para refletir essas mudanças.

### CSS-01.02 — Cascata, Especificidade e Herança

**Objetivo**

Compreender como o CSS **resolve conflitos** entre regras, determinar a especificidade de seletores e o papel da herança e da ordem das declarações.

**Fundamentos**

- **Cascata:** origem e ordem das regras (user agent, user, author) e o papel de `!important`.
- **Especificidade:** algoritmo que define peso de seletores (id > classe > elemento).
- **Herança:** propriedades que são herdadas (ex.: `color`, `font-family`) versus propriedades que não o são (ex.: `width`). Valores iniciais padrões.
- Como depurar conflitos comuns: declarar a mesma propriedade em regras diferentes, entender qual prevalece.

**Competências**

- Prever qual regra será aplicada quando múltiplas regras afetem o mesmo elemento/propriedade.
- Diagnosticar por que um estilo esperado não aparece (ex.: seletor errado, menor especificidade, ordem incorreta).
- Justificar decisões de estilo explicando origem, especificidade e herança das regras.
- Evitar hackeações simples, preferindo reorganizar CSS ou aumentar especificidade conscientemente.

**Dependências**

CSS-01.01 (conhecimento de seletores).

**Web Integration**

Resolver um problema de cascata em que diferentes arquivos CSS (ou estilos inline) definem a mesma propriedade. Ex.: um script JS alterna classes e o aluno explica por que o estilo resultante veio de uma regra específica (especificidade e ordem).

## Checklist

- [ ] Escrever seletores que atinjam exatamente os elementos desejados.
- [ ] Explicar qual regra CSS prevalece em caso de conflito (cascade + especificidade).
- [ ] Distinguir valores herdados dos valores iniciais e como isso afeta a estilização.
- [ ] Diagnosticar por que um estilo esperado não foi aplicado a um elemento.

## Validação do bloco

Ao final deste bloco, o aluno deve ser capaz de analisar um trecho de código CSS/HTML e explicar **por que** certa declaração (por exemplo, `color` ou `display`) está (ou não) sendo aplicada a um elemento, identificando a regra vencedora (considerando especificidade, origem e ordem) e se o valor veio por herança ou não.

---

# CSS-02 — Caixa e Dimensionamento

## Objetivo

Desenvolver compreensão do **modelo de caixa** do CSS e de como dimensões e unidades são calculadas. O aluno será capaz de controlar o tamanho real de elementos, espaçamentos e lidar com situações de overflow.

## Unidades

### CSS-02.01 — Modelo de Caixa (Box Model)

**Objetivo**

Entender que cada elemento é uma caixa composta por conteúdo, padding, borda e margem, e como ajustar esses valores.

**Fundamentos**

- Estrutura da caixa: conteúdo, `padding`, `border`, `margin`.
- Modelo de caixa padrão (`content-box`) vs `box-sizing: border-box`.
- Cálculo de largura/altura total de um elemento (por exemplo, `width` + padding + borda em *content-box*).
- Colapso de margens verticais (quando margens de elementos em bloco se fundem).
- Conceito de *containing block* para elementos relativos (relevante em posicionamento futuro).

**Competências**

- Calcular manualmente a largura/altura ocupada por um elemento, considerando padding e bordas.
- Usar `box-sizing` para alterar esse comportamento conforme necessidade.
- Ajustar margens e espaçamentos para manter alinhamentos previsíveis.
- Prever efeitos do colapso de margens em elementos sequenciais.

**Dependências**

CSS-01 (para aplicar estilos aos elementos certos).

**Web Integration**

Criar um “cartão” visual (card) onde se ajusta padding e margem para alinhar texto e imagem interna. Por exemplo, definir `box-sizing:border-box` para que o `width` defina o tamanho total do card, evitando overflow.

### CSS-02.02 — Valores, Unidades e Tipografia

**Objetivo**

Aprender sobre os diferentes tipos de valores e unidades no CSS e como escolher unidades relativas ou absolutas para tamanhos e espaçamentos.

**Fundamentos**

- Tipos de valores: numéricos, palavras-chave (ex.: `initial`, `inherit`) e funcionais (ex.: `calc()`).
- **Unidades absolutas:** `px`, `in`, `cm` (raramente usadas em web).
- **Unidades relativas:** `%`, `em`, `rem`, `vw`, `vh` etc.; entender referências de cálculo para cada uma.
- Importância de `em`/`rem` para escalabilidade de texto e layout (unidades relativas são mais acessíveis pois respeitam preferências do usuário).
- Uso de `%` para dimensões relativas ao elemento pai ou ao *containing block*.
- Unidades de cor (hexa, rgb(a), hsl(a)) e transparências básicas.

**Competências**

- Definir tamanhos de fonte, largura e espaço com unidades adequadas para tornar o layout flexível.
- Usar `rem` para fontes baseadas no tamanho raiz e `em` para espaçamentos dependentes de fonte atual.
- Converter unidades quando necessário (por exemplo, de px para rem).
- Reconhecer situações onde `percentage` facilita layouts fluidos.

**Dependências**

CSS-02.01 (para aplicar padding, largura etc.).

**Web Integration**

Implementar uma tipografia escalável: por exemplo, configurar `html { font-size: 100%; }` e usar `rem` para títulos, permitindo o ajuste proporcional se o usuário alterar o zoom/zoom da página.

### CSS-02.03 — Dimensões, Largura/Altura e Overflow

**Objetivo**

Controlar explicitamente as dimensões (width, height, min/max) de elementos e lidar com conteúdo que extrapola essas dimensões (overflow).

**Fundamentos**

- Propriedades `width`, `height`, `min-width`, `max-width`, `min-height`, `max-height` e como elas afetam o tamanho de boxes.
- Diferença entre valores fixos (px) e fluidos (% ou `auto`) nas dimensões.
- Comportamento do overflow: `overflow: visible/hidden/scroll/auto`. O que acontece quando o conteúdo não cabe (scrollbars, corte).
- Uso de `max-width: 100%` em imagens para evitar ultrapassar o contêiner (funda­mental para responsividade).

**Competências**

- Definir limites de tamanho (ex.: páginas centradas com `max-width` para legibilidade).
- Prever quando o conteúdo causará overflow e escolher estratégia (cortar, rolagem ou ajuste de layout).
- Aplicar porcentagens de forma que elementos se ajustem ao pai (ex.: colunas fluidas).
- Utilizar `box-sizing` (de 02.01) em conjunto para garantir que `width` inclua padding/borda conforme esperado.

**Dependências**

CSS-02.01, CSS-02.02.

**Web Integration**

Resolver um caso em que um painel de conteúdo está excedendo seu contêiner. Por exemplo, exibir barras de rolagem apenas quando necessário usando `overflow`, ou fazer imagens responsivas com `max-width: 100%`.

## Checklist

- [ ] Calcular o tamanho total de um elemento (incluindo padding e borda).
- [ ] Usar `box-sizing` para ajustar como o `width/height` são aplicados.
- [ ] Definir tamanhos usando unidades relativas (`%`, `em`, `rem`) quando quiser layout flexível.
- [ ] Prever e controlar overflow de conteúdo em contêineres.

## Validação do bloco

Ao final deste bloco, o aluno deve ser capaz de estruturar um layout simples (como um painel de texto ou cartão de produto) definindo larguras, alturas, margens e preenchimentos de maneira apropriada, justificando o uso de cada unidade e mostrando como resolver um eventual overflow. Por exemplo, explicar por que um elemento extrapola sua caixa e como ajustar `max-width` ou `overflow` para corrigir.

---

# CSS-03 — Fluxo Normal e Posicionamento

## Objetivo

Familiarizar-se com o **fluxo padrão** de layout do CSS e os principais mecanismos de posicionamento. O aluno aprenderá a prever como os elementos serão dispostos sem posicionamento especial, e como usar `position` para controlar localizações e sobreposições.

## Unidades

### CSS-03.01 — Fluxo normal (block vs inline) e display

**Objetivo**

Entender como elementos de bloco e inline são posicionados em fluxo normal e como as propriedades `display` controlam isso.

**Fundamentos**

- **Fluxo normal:** elementos em bloco (cada novo em linha) vs inline (no mesmo fluxo de linha).
- Propriedade `display`: valores básicos `block`, `inline`, `inline-block`, `none`, e noções de `flex`/`grid` como display (introdução).
- Colapso de margem entre elementos de bloco adjacentes.
- **Espaçamento branco (white-space)** e quebra automática de linha em texto inline.
- Conceito de *containing block* no contexto de elementos posicionados (ligado a fluxo).

**Competências**

- Prever a posição inicial de elementos (por ex., duas `div` em sequência ficam empilhadas).
- Usar `display` para alterar o comportamento padrão (transformar bloco em inline-block, esconder elementos).
- Solucionar problemas de layout relacionados ao fluxo, como espaços indesejados entre elementos inline-block.
- Diferenciar `visibility: hidden` de `display: none` (impacto no fluxo).

**Dependências**

CSS-02.

**Web Integration**

Ajustar o layout de um cabeçalho com itens de menu: tornar elementos `li` em linha (`display:inline-block`) ou em bloco horizontal, garantindo que se comportem como desejado no fluxo.

### CSS-03.02 — Posicionamento Estático e Relativo

**Objetivo**

Aprender os efeitos de `position: static` (padrão) e `position: relative` em elementos.

**Fundamentos**

- Posição estática: o elemento permanece no fluxo normal (padrão).
- `position: relative`: desloca um elemento em relação à sua posição original sem removê-lo do fluxo (ex.: `left: 10px` desloca, mas espaço original é mantido).
- `top/right/bottom/left` em elementos relativos (movimentação a partir da posição inicial).
- Conceito básico de *containing block* para elementos relativamente posicionados (normalmente, o próprio elemento).
- Origem do sistema de coordenadas local para offsets.

**Competências**

- Ajustar local rapidamente um elemento em relação à sua posição natural (ex.: criar um alinhamento fino).
- Prever como um `position: relative` afetará o layout (outro conteúdo não reposiciona totalmente).
- Usar deslocamentos sem quebrar o fluxo geral da página.

**Dependências**

CSS-03.01.

**Web Integration**

Posicionar um elemento de destaque levemente deslocado (por exemplo, um selo “New” sobre um banner) usando `position: relative` no elemento pai e `position: absolute` no selo (a ser visto em posicionamento absoluto). No contexto deste exercício, o foco será entender o deslocamento relativo antes de usar absoluto.

### CSS-03.03 — Posicionamento Absoluto, Fixo, Sticky e Empilhamento

**Objetivo**

Aprender como remover elementos do fluxo e posicioná-los de forma independente, e como controlar a ordem de empilhamento (z-index).

**Fundamentos**

- `position: absolute`: elemento sai do fluxo normal; posicionado em relação ao *containing block* (o ancestral posicionado mais próximo).
- `position: fixed`: elemento fixo em relação à viewport (sempre visível no mesmo lugar da tela).
- `position: sticky`: comportamento híbrido (posiciona como estático até certo ponto de scroll, depois se fixa).
- Como definir `top/right/bottom/left` nesses casos para posicionar o elemento precisamente.
- **Stacking context:** `z-index` define a ordem de sobreposição em contexto de empilhamento (possuem contexto elementos posicionados ou raiz); elementos com maior z-index aparecem na frente.

**Competências**

- Colocar elementos em camadas sobrepostos de forma controlada (ex.: menus ou modais) usando `z-index`.
- Usar `position: absolute` para criar sobreposições, painéis popup ou ícones posicionados (ex.: texto sobre imagem).
- Entender como `fixed` garante barras fixas no topo/rodapé independente do scroll.
- Identificar *containing block* de um elemento absoluto (pai posicionado).

**Dependências**

CSS-03.01, CSS-03.02.

**Web Integration**

Construir um menu fixo no topo da página (`fixed`) ou uma caixa de diálogo posicionada (`absolute`) sobre o conteúdo; por exemplo, um modal ou tooltip que requer posicionamento fora do fluxo normal.

### CSS-03.04 — Floats e Layout Legado (conteúdo opcional)

**Objetivo**

Compreender o uso original da propriedade `float` e seu impacto no fluxo (técnicas legadas de layout).

**Fundamentos**

- `float: left/right`: tira o elemento do fluxo de texto normal e faz o texto fluir ao redor dele (como no layout de imagem com texto contornando).
- Problemas de *clear* (limpeza): quando elementos subsequentes podem fluir para o lado do *float*, uso de `clear: both` para quebrar o fluxo.
- Uso histórico de floats para criar layouts de colunas antes do flex/grid (técnica legada).

**Competências**

- Aplicar float em elementos para fazer texto contornar (como imagens em parágrafos).
- Resolver colapsos de altura em contêineres que têm apenas filhos flutuantes (ex.: clearfix).
- Reconhecer quando não usar float em layouts modernos (preferir flex/grid para colunas).

**Dependências**

CSS-03.01.

**Web Integration**

Flutuar uma imagem à esquerda de um parágrafo, garantindo que o texto se ajuste corretamente (float). Em um contexto de integração, adicionar clareza de funcionamento comparando com Flexbox para colunas como alternativa.

## Checklist

- [ ] Prever como dois elementos de bloco ou inline aparecem no fluxo normal.
- [ ] Usar `display` para modificar o comportamento de elementos (por exemplo, `inline-block` vs `block`).
- [ ] Posicionar um elemento relativo para ajustes finos sem tirar do fluxo.
- [ ] Remover um elemento do fluxo usando `position: absolute/fixed` e controlá-lo com `z-index`.
- [ ] Compreender e evitar armadilhas de floats (e limpá-los com `clear` quando necessário).

## Validação do bloco

Ao final deste bloco, o aluno deve ser capaz de reconstruir um layout estático complexo, explicando como cada elemento se posiciona: distinguir qual está no fluxo normal, qual foi movido por `position`, e como o `z-index` determina camadas de sobreposição. Por exemplo, justificar o uso de `absolute` sobre uma imagem de fundo para posicionar texto ou a conversão de elementos em `inline-block` para alinhamento horizontal.

---

# CSS-04 — Layout com Flexbox e Grid

## Objetivo

Desenvolver a capacidade de escolher e usar corretamente **Flexbox e CSS Grid** para resolver problemas de layout complexos. O aluno aprenderá a analisar um problema de layout (dimensionalidade, relação entre itens) e aplicar o sistema de layout adequado, controlando eixo, alinhamento e espaço disponível.

## Unidades

### CSS-04.01 — Flexbox (Layout Unidimensional)

**Objetivo**

Entender o **modelo flexbox**, dispondo itens em um único eixo (linha ou coluna) de maneira flexível.

**Fundamentos**

- Contêiner flexível (`display: flex` ou `inline-flex`) e flex items (filhos diretos).
- Eixos do flexbox: eixo principal (main axis) e cruzado (cross axis).
- Propriedades do contêiner: `flex-direction` (row/column), `flex-wrap` (embrulhar ou não), `justify-content` (distribuição no eixo principal), `align-items` (alinhamento no eixo cruzado).
- Propriedades dos itens: `flex-grow`, `flex-shrink`, `flex-basis` (dimensões flexíveis), alinhamento individual (`align-self`).
- Ordenação de itens (`order`) e impactos.

**Competências**

- Criar colunas ou filas iguais facilmente (por exemplo, 3 cards lado a lado que se expandem igualmente).
- Centralizar itens no eixo principal ou cruzado sem ajustes de margem.
- Resolver excesso de conteúdo usando `flex-wrap`.
- Comparar cenários: **quando usar flexbox** em vez de grid ou fluxo normal (situações 1D, filas flexíveis).

**Dependências**

CSS-03.

**Web Integration**

Implementar um layout de “cards” onde cada linha deve conter um número variável de itens que se ajustam ao espaço. Por exemplo, um cabeçalho com itens de navegação distribuidos uniformemente no eixo principal, ou uma galeria responsiva de cartões usando `flex`.

### CSS-04.02 — CSS Grid (Layout Bidimensional)

**Objetivo**

Entender o **modelo Grid**, criando layouts em linhas e colunas simultaneamente.

**Fundamentos**

- Contêiner de grade (`display: grid` ou `inline-grid`) e grid items.
- Definição de linhas e colunas com `grid-template-rows/columns` ou `grid-template-areas`.
- Grelha implícita vs definida: `grid-auto-flow`, `auto-fill/repeat()` com unidades `fr`.
- Espaçamento: `gap`, `row-gap`, `column-gap`.
- Alinhamento dentro de grid: `justify-items`, `align-items`, `justify-content`, `align-content`.

**Competências**

- Construir layouts complexos de duas dimensões (por exemplo, painéis com cabeçalho lateral e conteúdos alinhados em grade).
- Posicionar itens em células específicas ou áreas nomeadas.
- Combinar unidades fixas e flexíveis (`fr`) para controlar proporção de colunas/linhas.
- Saber quando **Grid** é mais adequado que Flexbox (problemas 2D, definição explícita de áreas).

**Dependências**

CSS-04.01 (compreensão prévia de flex ajuda, mas não estritamente necessária).

**Web Integration**

Criar a estrutura de página com cabeçalho, menu lateral e conteúdo principal usando Grid. Por exemplo, definir uma grade 2x2 onde o cabeçalho ocupa toda a largura e o menu ocupa a coluna esquerda em múltiplas linhas.

## Checklist

- [ ] Construir layouts de uma linha ou coluna com Flexbox (centralizando e distribuindo espaço).
- [ ] Construir layouts mais complexos em grelha (2D) com CSS Grid.
- [ ] Explicar por que escolhi Flexbox ou Grid para um certo problema de layout.
- [ ] Usar propriedades de alinhamento (`justify`/`align`) em flex ou grid para posicionar itens.

## Validação do bloco

Ao final deste bloco, o aluno deve conseguir montar um layout de página completo utilizando Flexbox e Grid de forma combinada. Por exemplo, justificar o uso de Grid para a estrutura geral e Flexbox para componentes internos (ou vice-versa), explicando como cada sistema distribui espaço e alinha itens no caso específico. Deverá diagnosticar resultados inesperados, como item que excede a área da grelha ou não se alinha, ajustando as propriedades adequadas.

---

# CSS-05 — Responsividade e Adaptação

## Objetivo

Preparar o aluno para criar interfaces que **se adaptam a diferentes dispositivos**, usando layouts fluidos e consultas de mídia. O foco é entender como o design pode ser flexível em vez de fixo.

## Unidades

### CSS-05.01 — Layout Fluido e Unidades Relativas

**Objetivo**

Dominar técnicas para fazer componentes dimensionais fluírem com o tamanho da tela ou contêiner.

**Fundamentos**

- Layout líquido: definir larguras com `%`, `vw`, `vh` para preencher contêineres fluentes.
- Uso de `max-width` para limitar crescimento (ex.: evitar que texto fique muito largo).
- Imagens e mídias fluídas: `img { max-width: 100%; height: auto; }` para redimensionar imagens dentro do contêiner.
- Unidades de viewport (`vw`, `vh`) para font-size ou larguras relativas ao tamanho da janela.
- Conceito de tipografia responsiva: `clamp()`, tamanhos base em `rem` e espaçamento proporcional.

**Competências**

- Criar colunas que se redimensionam (porcentagens em `width`).
- Garantir que mídias (imagens, vídeos) nunca ultrapassem seus contêineres.
- Evitar layout fixo em pixels, preferindo unidades flexíveis.
- Antecipar como elementos redimensionam quando a janela muda de tamanho.

**Dependências**

CSS-02 (unidades).

**Web Integration**

Construir um grid responsivo onde as colunas crescem/encolhem conforme o navegador; ajustar imagens e textos para que redimensionem sem distorção, mantendo proporção e legibilidade.

### CSS-05.02 — Media Queries e Breakpoints

**Objetivo**

Aprender a usar *Media Queries* para alterar estilos conforme condições (largura, orientação, resolução).

**Fundamentos**

- Sintaxe das media queries (`@media (min-width: X)` etc.) e tipos de mídia (screen, print).
- Estratégia mobile-first: escrever CSS base para mobile e usar `min-width` para grandes telas.
- Definir breakpoints: identificar larguras em que o layout deve mudar.
- Adaptação de layout: reorganizar colunas em linhas, esconder/mostrar elementos, alterar tamanhos em diferentes faixas de tela.
- Conceito de *design adaptativo* vs *responsivo*.

**Competências**

- Escrever regras CSS condicionais para diferentes tamanhos de viewport.
- Escolher breakpoints baseados no design (ex.: quando o conteúdo começa a ficar apertado).
- Testar no navegador usando ferramentas de desenvolvedor (alternância de dimensões).
- Justificar a escolha de um ponto de quebra específico com base na fluidez do conteúdo.

**Dependências**

CSS-05.01.

**Web Integration**

Implementar um design de site onde em telas estreitas (mobile) os itens ficam empilhados verticalmente, e em telas largas formam colunas horizontais. Exemplo: converter um menu de hambúrguer em barras horizontais via media query.

## Checklist

- [ ] Fazer um layout escalar com percentuais e unidades flexíveis, sem usar larguras fixas em pixels.
- [ ] Configurar *media queries* para reorganizar o layout em diferentes larguras.
- [ ] Garantir que imagens e textos sejam redimensionados adequadamente (ex.: `max-width:100%`).
- [ ] Implementar uma abordagem *mobile-first*, aplicando estilos mobile e expandindo para desktop via media queries.

## Validação do bloco

Ao final deste bloco, o aluno deve demonstrar uma interface totalmente *responsiva*: por exemplo, uma página que muda de 3 colunas para 1 coluna em telas pequenas. Ele deve explicar como usou unidades fluídas e media queries para cada adaptação, justificando pontos de quebra baseados no conteúdo visível. Deve diagnosticar o que causa overflow ou quebra de layout em diferentes larguras e corrigi-los.

---

# CSS-06 — Acessibilidade e Qualidade de Layout

## Objetivo

Incorporar **considerações de acessibilidade** nas decisões de CSS, garantindo interfaces claras e utilizáveis. O aluno entenderá como escolhas de estilo afetam legibilidade, contraste e navegabilidade, promovendo um design inclusivo.

## Unidades

### CSS-06.01 — Tipografia e Legibilidade

**Objetivo**

Garantir textos legíveis e interface limpa, usando tamanhos e espaçamentos adequados.

**Fundamentos**

- Tamanho de fonte mínimo recomendado (ex.: ≥ 16px padrão) e uso de `line-height` para facilitar leitura.
- Unidades relativas para texto (`em`, `rem`) que respeitam configurações do usuário.
- Contraste de cores: importância de combinar fundo/primeiro plano com boa legibilidade (evitar texto claro em fundo claro, alcançar razão de contraste razoável).
- Espaçamento: distância adequada entre linhas e parágrafos para facilitar leitura contínua.

**Competências**

- Definir tamanhos de fonte e espaçamentos de forma escalável e ajustável.
- Escolher cores ou filtros de contraste para manter legibilidade (por exemplo, não usar cinza muito claro em texto de parágrafo).
- Explicar como diferentes tamanhos e contrastes impactam usuários com baixa visão.
- Aplicar estilos tipográficos que se ajustem a ampliação de tela sem sobrecarga do layout.

**Dependências**

CSS-02 (unidades e dimensões).

**Web Integration**

Revisar um design de formulário ou artigo e ajustar tamanhos de fonte/unidades para torná-los responsivos a configurações de zoom do navegador.

### CSS-06.02 — Estados de Interação e Foco

**Objetivo**

Manter interfaces navegáveis por teclado e indicadores visuais claros (hover, foco, ativo).

**Fundamentos**

- Estilos de hover e active (`:hover`, `:active`); realce de itens interativos.
- Indicador de foco (`:focus` ou `:focus-visible`): manter ou estilizar outline padrão para acessibilidade.
- Nunca remover completamente os estilos de foco (outline), pois isso prejudica usuários de teclado.
- Tamanho adequado de áreas clicáveis (paddings mínimos em botões ou links).

**Competências**

- Assegurar que elementos interativos mostram estado visível quando focados via teclado.
- Diferenciar `:hover` (mouse) de `:focus` (teclado) e usar `:focus-visible` quando apropriado.
- Criar estilos evidentes (cores ou contornos) que indiquem foco, atendendo aos critérios de usabilidade.
- Evitar usar apenas cor para transmitir informação (ex.: “estilos importantes” usando cor + outro indicador).

**Dependências**

CSS-01 (pseudoclasses).

**Web Integration**

Desenvolver um menu de navegação acessível que mostra outline nos links ao receber foco por Tab, e destacar o item atual via `:focus`.

### CSS-06.03 — Ocultamento e Ordens de Leitura

**Objetivo**

Ocultar elementos de forma adequada sem prejudicar leitores de tela, e manter ordem lógica de conteúdo.

**Fundamentos**

- `display: none` remove do fluxo e também da árvore de acessibilidade (conteúdo não é lido por leitores de tela).
- `visibility: hidden` esconde visualmente mas mantém espaço no layout; leitores de tela ainda verão o conteúdo (discutir quando usar cada um).
- Posicionamentos fora de tela (ex.: `position: absolute; left: -9999px`) para esconder conteúdo de layout mas mantê-lo disponível (ex.: texto alternativo).
- Leitura de conteúdo na ordem do DOM: mesmo que CSS reordene visualmente, manter estrutura HTML semântica (flex/grid não devem reordenar mentalmente o conteúdo sem necessidade).

**Competências**

- Decidir como esconder conteúdo (por ex., menus móveis) sem quebrar acessibilidade.
- Garantir que a ordem de foco (tab order) segue o fluxo visual ou está clara.
- Justificar o uso de `display:none` vs outras técnicas para esconder conteúdo dinâmico.

**Dependências**

CSS-03 (fluxo e posicionamento).

**Web Integration**

Criar um menu “off-canvas” que aparece ao clicar num botão: usar `display:none` e depois `display:block` via CSS/JS, assegurando que o conteúdo escondido não confunda leitores de tela.

## Checklist

- [ ] Escolher tamanhos de fonte e espaçamentos que mantenham a legibilidade (usar unidades proporcionais).
- [ ] Garantir contraste suficiente entre texto e fundo (evitar combinações ilegíveis).
- [ ] Manter indicadores de foco visíveis em elementos interativos (não remover o outline padrão).
- [ ] Ocultar elementos sem quebrar o fluxo de leitura para tecnologias assistivas.

## Validação do bloco

Ao final deste bloco, o aluno deverá avaliar e corrigir um exemplo de interface simple para torná-lo acessível. Por exemplo, ao explicar um layout com botões e links, ele apontará problemas de contraste ou falta de foco visível, mostrando como ajustes no CSS (tamanhos relativos, outline, etc.) resolvem esses problemas sem alterar o HTML estrutural.

---

### Navegação

[← Mapa curricular](./README.md) ·
[↑ CSS Foundations Lab](../README.md) ·
[CSS-01 — Seletores, Especificidade e Cascata →](../practice/css-01-seletores-especificidade-e-cascata/)
