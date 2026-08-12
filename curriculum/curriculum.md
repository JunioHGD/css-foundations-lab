# CSS Lab

## Identificação

**Lab:** CSS Lab

**Sigla:** CSS

**Finalidade:** Construir uma base que permita compreender e prever o comportamento do CSS, selecionar conscientemente seus mecanismos de layout, criar interfaces responsivas e acessíveis e adquirir recursos posteriores sem precisar reaprender os modelos fundamentais da linguagem.

---

# Estrutura curricular

## CSS-01 — Regras, seleção e resolução de estilos

### Objetivo

Compreender como CSS associa declarações aos elementos e determina quais valores efetivamente participam da renderização.

### Unidades

#### CSS-01.01 — Estrutura da linguagem e aplicação de estilos

**Objetivo:** compreender a composição mínima de uma folha de estilos e sua relação com o documento.

**Conceitos fundamentais:**

1. CSS como linguagem de apresentação de documentos estruturados;
2. folhas de estilo;
3. regras de estilo;
4. seletores;
5. blocos de declarações;
6. propriedades e valores;
7. declarações válidas, inválidas e valores não suportados.

**Chats derivados:**

- `CSS-01.01 — Estudo — Estrutura da linguagem e aplicação de estilos`
- `CSS-01.01 — Prática — Estrutura da linguagem e aplicação de estilos`

#### CSS-01.02 — Seletores, relações e estados

**Objetivo:** selecionar elementos segundo identidade, estrutura, relação e estado sem misturar seleção com comportamento programático.

**Conceitos fundamentais:**

1. seletores de tipo, classe, ID, atributo e universal;
2. seletores compostos e listas de seletores;
3. combinadores e relações estruturais;
4. pseudo-classes;
5. estados de interação, incluindo foco;
6. pseudo-elementos;
7. relação entre escolha de seletor e especificidade.

**Chats derivados:**

- `CSS-01.02 — Estudo — Seletores, relações e estados`
- `CSS-01.02 — Prática — Seletores, relações e estados`

#### CSS-01.03 — Cascata, especificidade e herança

**Objetivo:** prever qual declaração vence quando diferentes regras podem determinar o mesmo valor.

**Conceitos fundamentais:**

1. relevância das declarações;
2. origens da cascata;
3. importância normal e `!important`;
4. camadas de cascata;
5. especificidade;
6. ordem de aparecimento;
7. herança;
8. valores iniciais e valores herdados;
9. palavras-chave globais de controle da cascata;
10. progressão entre valor declarado, cascaded, specified, computed e used.

**Chats derivados:**

- `CSS-01.03 — Estudo — Cascata, especificidade e herança`
- `CSS-01.03 — Prática — Cascata, especificidade e herança`

#### CSS-01.04 — Valores, unidades e custom properties

**Objetivo:** compreender como valores expressam dimensões, relações e cálculos e como podem ser reutilizados pela própria cascata.

**Conceitos fundamentais:**

1. tipos de valores CSS e leitura básica da sintaxe de valores;
2. números, comprimentos e ângulos;
3. unidades absolutas e relativas;
4. `em` e `rem`;
5. porcentagens e seus valores de referência;
6. unidades relativas ao viewport;
7. funções matemáticas fundamentais: `calc()`, `min()`, `max()` e `clamp()`;
8. custom properties;
9. `var()` e valores de fallback;
10. cascata e herança das custom properties.

**Chats derivados:**

- `CSS-01.04 — Estudo — Valores, unidades e custom properties`
- `CSS-01.04 — Prática — Valores, unidades e custom properties`

### Resultado esperado

O estudante consegue explicar **por que determinado valor foi aplicado a determinado elemento** e trabalhar com a cascata sem depender de tentativa e erro.

### Checkpoint derivado

`CSS-01 — Checkpoint — Regras, seleção e resolução de estilos`

---

## CSS-02 — Apresentação, caixas e fluxo

### Objetivo

Compreender como conteúdo estilizado gera caixas, ocupa espaço e participa do fluxo e do sistema de coordenadas do documento.

### Unidades

#### CSS-02.01 — Cor, texto e tipografia fundamentais

**Objetivo:** controlar as características visuais essenciais que influenciam legibilidade e dimensionamento do conteúdo.

**Conceitos fundamentais:**

1. cor de primeiro plano e de fundo;
2. valores de cor e transparência;
3. famílias tipográficas e fallbacks;
4. tamanho, peso e estilo da fonte;
5. altura de linha;
6. alinhamento e decoração textual;
7. quebra, espaços e fluxo básico do texto.

**Chats derivados:**

- `CSS-02.01 — Estudo — Cor, texto e tipografia fundamentais`
- `CSS-02.01 — Prática — Cor, texto e tipografia fundamentais`

#### CSS-02.02 — Modelo de caixa

**Objetivo:** compreender como as dimensões visíveis e o espaço ocupado por um elemento são formados.

**Conceitos fundamentais:**

1. content box;
2. padding;
3. border;
4. margin;
5. `content-box` e `border-box`;
6. `box-sizing`;
7. cálculo da dimensão total da caixa;
8. colapso de margens no fluxo em bloco;
9. backgrounds e borders como decoração da caixa.

**Chats derivados:**

- `CSS-02.02 — Estudo — Modelo de caixa`
- `CSS-02.02 — Prática — Modelo de caixa`

#### CSS-02.03 — Display, fluxo e dimensionamento

**Objetivo:** compreender como caixas participam do fluxo e como seus tamanhos são determinados e limitados.

**Conceitos fundamentais:**

1. geração de caixas e `display`;
2. tipos externos e internos de display;
3. comportamento block e inline;
4. fluxo normal;
5. caixas in-flow e relações com o conteúdo;
6. eixos block e inline;
7. dimensões físicas e propriedades lógicas;
8. `auto` e espaço disponível;
9. porcentagens e containing block;
10. dimensões mínimas e máximas;
11. dimensionamento intrínseco: `min-content`, `max-content` e `fit-content`;
12. conteúdo substituído e dimensões intrínsecas;
13. overflow e scroll containers.

**Chats derivados:**

- `CSS-02.03 — Estudo — Display, fluxo e dimensionamento`
- `CSS-02.03 — Prática — Display, fluxo e dimensionamento`

#### CSS-02.04 — Posicionamento e empilhamento

**Objetivo:** compreender quando uma caixa permanece no fluxo, quando é deslocada e em relação a qual referência suas coordenadas são calculadas.

**Conceitos fundamentais:**

1. containing block;
2. `position: static`;
3. posicionamento relativo;
4. posicionamento absoluto;
5. posicionamento fixo;
6. posicionamento sticky;
7. inset e offsets;
8. participação e remoção do fluxo;
9. eixo de profundidade;
10. `z-index`;
11. stacking contexts e ordem de pintura.

**Chats derivados:**

- `CSS-02.04 — Estudo — Posicionamento e empilhamento`
- `CSS-02.04 — Prática — Posicionamento e empilhamento`

### Resultado esperado

O estudante consegue prever **quanto espaço uma caixa ocupa, onde ela será posicionada e como o conteúdo ao redor reagirá**, inclusive diante de restrições e overflow.

### Checkpoint derivado

`CSS-02 — Checkpoint — Apresentação, caixas e fluxo`

---

## CSS-03 — Sistemas de layout e adaptação

### Objetivo

Aprender a escolher e combinar os sistemas modernos de layout em vez de utilizar posicionamento ou propriedades isoladas como soluções genéricas.

### Unidades

#### CSS-03.01 — Eixos, alinhamento e escolha do mecanismo

**Objetivo:** reconhecer o problema de layout antes de selecionar a ferramenta que irá resolvê-lo.

**Conceitos fundamentais:**

1. fluxo normal como comportamento inicial;
2. distribuição versus posicionamento;
3. eixos block/inline e main/cross;
4. alinhamento de itens e conteúdo;
5. distribuição de espaço disponível;
6. `gap`;
7. alinhamento coletivo e individual;
8. diferença conceitual entre fluxo, posicionamento, Flexbox e Grid.

**Chats derivados:**

- `CSS-03.01 — Estudo — Eixos, alinhamento e escolha do mecanismo`
- `CSS-03.01 — Prática — Eixos, alinhamento e escolha do mecanismo`

#### CSS-03.02 — Flexbox

**Objetivo:** construir layouts em que a distribuição e o alinhamento ocorram principalmente ao longo de um eixo.

**Conceitos fundamentais:**

1. flex container e flex items;
2. main axis e cross axis;
3. direção;
4. flex lines e wrapping;
5. flex basis;
6. crescimento e encolhimento;
7. distribuição de espaço;
8. alinhamento nos dois eixos;
9. gaps;
10. implicações da reordenação visual.

**Chats derivados:**

- `CSS-03.02 — Estudo — Flexbox`
- `CSS-03.02 — Prática — Flexbox`

#### CSS-03.03 — Grid

**Objetivo:** construir layouts nos quais linhas e colunas precisam ser controladas conjuntamente.

**Conceitos fundamentais:**

1. grid container e grid items;
2. linhas, tracks, células e áreas;
3. linhas e colunas;
4. grid explícito e implícito;
5. tamanhos fixos, flexíveis e unidade `fr`;
6. `minmax()` e `repeat()` como instrumentos do modelo de tracks;
7. posicionamento por linhas e áreas;
8. auto-placement;
9. alinhamento;
10. gaps;
11. sobreposição de itens;
12. diferença de responsabilidade entre Grid e Flexbox.

**Chats derivados:**

- `CSS-03.03 — Estudo — Grid`
- `CSS-03.03 — Prática — Grid`

#### CSS-03.04 — Layout responsivo e Media Queries

**Objetivo:** produzir layouts que se adaptem ao espaço disponível e às características relevantes do ambiente.

**Conceitos fundamentais:**

1. layout fluido como comportamento preferencial;
2. dimensionamento relativo e restrições;
3. Flexbox e Grid responsivos;
4. media queries;
5. media features;
6. consultas por largura, altura e orientação;
7. range queries;
8. breakpoints determinados pela necessidade do layout;
9. estratégias mobile-first e suas limitações;
10. combinação entre adaptação fluida e mudanças condicionais.

**Chats derivados:**

- `CSS-03.04 — Estudo — Layout responsivo e Media Queries`
- `CSS-03.04 — Prática — Layout responsivo e Media Queries`

### Resultado esperado

O estudante consegue escolher entre fluxo, posicionamento, Flexbox e Grid e compor interfaces que **se reorganizam pelo comportamento do conteúdo e do espaço disponível**, em vez de depender de dimensões rígidas.

### Checkpoint derivado

`CSS-03 — Checkpoint — Sistemas de layout e adaptação`

---

## CSS-04 — Robustez, acessibilidade e organização

### Objetivo

Garantir que o CSS produzido continue compreensível, previsível e utilizável diante de diferentes usuários, tamanhos de viewport e necessidades de interação.

### Unidades

#### CSS-04.01 — Acessibilidade visual e de interação no CSS

**Objetivo:** estilizar interfaces sem remover ou prejudicar informações e mecanismos de interação necessários ao usuário.

**Conceitos fundamentais:**

1. contraste de texto e componentes;
2. informação não transmitida exclusivamente por cor;
3. foco visível;
4. foco não obscurecido por elementos sobrepostos;
5. legibilidade e espaçamento textual;
6. redimensionamento de texto;
7. zoom e reflow;
8. prevenção de overflow horizontal desnecessário;
9. ordem visual versus ordem estrutural;
10. preservação da ordem de navegação;
11. movimento e `prefers-reduced-motion`;
12. media queries relacionadas a preferências do usuário.

**Chats derivados:**

- `CSS-04.01 — Estudo — Acessibilidade visual e de interação no CSS`
- `CSS-04.01 — Prática — Acessibilidade visual e de interação no CSS`

#### CSS-04.02 — Organização nativa e controle da cascata

**Objetivo:** manter folhas de estilo extensíveis sem introduzir complexidade metodológica externa prematuramente.

**Conceitos fundamentais:**

1. classes reutilizáveis e seletores com responsabilidade clara;
2. especificidade previsível;
3. preferência por cascata controlada em vez de escalada de especificidade;
4. uso deliberado da ordem das regras;
5. uso consciente de cascade layers;
6. uso excepcional, e não rotineiro, de `!important`;
7. custom properties para valores compartilhados e configuração local;
8. escopo natural das custom properties pela árvore;
9. agrupamento coerente de regras;
10. nomenclatura consistente sem dependência de metodologia específica.

**Chats derivados:**

- `CSS-04.02 — Estudo — Organização nativa e controle da cascata`
- `CSS-04.02 — Prática — Organização nativa e controle da cascata`

### Resultado esperado

O estudante consegue produzir CSS cuja apresentação continua utilizável em diferentes condições e cuja cascata permanece suficientemente controlada para crescimento posterior.

### Checkpoint derivado

`CSS-04 — Checkpoint — Robustez, acessibilidade e organização`

---

# Mapa operacional dos chats

```text
CSS-01 — Regras, seleção e resolução de estilos

CSS-01.01 — Estudo — Estrutura da linguagem e aplicação de estilos
CSS-01.01 — Prática — Estrutura da linguagem e aplicação de estilos

CSS-01.02 — Estudo — Seletores, relações e estados
CSS-01.02 — Prática — Seletores, relações e estados

CSS-01.03 — Estudo — Cascata, especificidade e herança
CSS-01.03 — Prática — Cascata, especificidade e herança

CSS-01.04 — Estudo — Valores, unidades e custom properties
CSS-01.04 — Prática — Valores, unidades e custom properties

CSS-01 — Checkpoint — Regras, seleção e resolução de estilos

CSS-02 — Apresentação, caixas e fluxo

CSS-02.01 — Estudo — Cor, texto e tipografia fundamentais
CSS-02.01 — Prática — Cor, texto e tipografia fundamentais

CSS-02.02 — Estudo — Modelo de caixa
CSS-02.02 — Prática — Modelo de caixa

CSS-02.03 — Estudo — Display, fluxo e dimensionamento
CSS-02.03 — Prática — Display, fluxo e dimensionamento

CSS-02.04 — Estudo — Posicionamento e empilhamento
CSS-02.04 — Prática — Posicionamento e empilhamento

CSS-02 — Checkpoint — Apresentação, caixas e fluxo

CSS-03 — Sistemas de layout e adaptação

CSS-03.01 — Estudo — Eixos, alinhamento e escolha do mecanismo
CSS-03.01 — Prática — Eixos, alinhamento e escolha do mecanismo

CSS-03.02 — Estudo — Flexbox
CSS-03.02 — Prática — Flexbox

CSS-03.03 — Estudo — Grid
CSS-03.03 — Prática — Grid

CSS-03.04 — Estudo — Layout responsivo e Media Queries
CSS-03.04 — Prática — Layout responsivo e Media Queries

CSS-03 — Checkpoint — Sistemas de layout e adaptação

CSS-04 — Robustez, acessibilidade e organização

CSS-04.01 — Estudo — Acessibilidade visual e de interação no CSS
CSS-04.01 — Prática — Acessibilidade visual e de interação no CSS

CSS-04.02 — Estudo — Organização nativa e controle da cascata
CSS-04.02 — Prática — Organização nativa e controle da cascata

CSS-04 — Checkpoint — Robustez, acessibilidade e organização

CSS — Checkpoint Final
```

# Competências ao concluir o Lab

1. **Explicar e prever** por que determinada declaração CSS é aplicada.
2. **Raciocinar sobre valores, unidades, herança e dimensionamento** sem depender apenas de tentativa e erro.
3. **Prever o comportamento de caixas**, fluxo, overflow, containing blocks e empilhamento.
4. **Escolher conscientemente** entre fluxo normal, posicionamento, Flexbox e Grid.
5. **Construir layouts fluidos e responsivos**, utilizando media queries somente quando necessárias.
6. **Preservar requisitos fundamentais de acessibilidade** relacionados à apresentação e interação.
7. **Estruturar CSS com cascata e especificidade previsíveis**, mantendo possibilidade de crescimento.
8. **Ler documentação e especificações posteriormente** e incorporar novas propriedades sem reconstruir os modelos mentais fundamentais.

# Aprofundamentos posteriores

- **Seleção e cascata avançadas:** `:is()`, `:where()`, `:has()`, `@scope`, nesting nativo e técnicas avançadas com cascade layers.
- **Custom properties avançadas:** `@property`, propriedades tipadas e padrões mais sofisticados de composição.
- **Layout especializado:** `subgrid`, container queries, multicolumn layout, layouts de tabelas e técnicas avançadas de dimensionamento.
- **Posicionamento especializado:** anchor positioning, posicionamento avançado e casos complexos de stacking contexts.
- **Movimento e efeitos:** transforms, transitions, animations, filters, clipping, masking e blending.
- **Cor e apresentação avançadas:** espaços de cor modernos, interpolação, gradientes, múltiplos backgrounds e efeitos gráficos.
- **Tipografia avançada:** `@font-face`, variable fonts, OpenType, color fonts e controles tipográficos especializados.
- **Outros meios:** impressão, paged media e estilos específicos para diferentes meios.
- **Legado e interoperabilidade:** `float` em seu papel atual de envolvimento de conteúdo, `clear`, clearfix, manutenção de layouts antigos baseados em floats/tabelas e hacks históricos. Como sistema geral de layout de página, floats e tabelas foram superados por modelos concebidos especificamente para esse problema, sobretudo Flexbox e Grid.
- **Arquitetura e tooling:** BEM, OOCSS, SMACSS, Sass, Less, PostCSS, CSS Modules, CSS-in-JS, frameworks e pipelines de build.
- **Acessibilidade ampliada:** estudo sistemático da WCAG e dos aspectos semânticos e comportamentais pertencentes a HTML e JavaScript.
