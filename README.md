# Base Site

Este é um projeto base para a criação de sites utilizando HTML, CSS, SASS e JavaScript puros. O objetivo é fornecer uma estrutura inicial organizada e bem documentada para acelerar o desenvolvimento de novos projetos web.

## Estrutura de Arquivos

```
/
├── css/
│   ├── sass/
│   │   ├── _colors.scss
│   │   ├── _layout.scss
│   │   ├── _spacing.scss
│   │   └── _typography.scss
│   ├── style.css
│   ├── style.css.map
│   └── style.scss
├── js/
│   └── svg-inject.min.js
├── svg/
├── index.html
└── README.md
```

## Descrição dos Arquivos e Diretórios

### `index.html`

O arquivo HTML principal. Ele contém a estrutura básica de uma página web, incluindo:
- Meta tags para SEO, redes sociais e configuração de viewport.
- Link para a folha de estilos principal (`css/style.css`).
- Inclusão do script `svg-inject.min.js` para manipulação de SVGs.

### `css/`

Este diretório contém todos os arquivos relacionados ao estilo do site.

#### `style.scss`

É o arquivo SASS principal. Ele é responsável por importar todos os outros arquivos SASS (parciais) e compilá-los em um único arquivo CSS (`style.css`).

#### `sass/`

Este subdiretório contém os arquivos parciais SASS, que dividem o estilo em seções lógicas:

- **`_colors.scss`**: Define a paleta de cores do projeto (cores primárias, secundárias, neutras, etc.) e classes utilitárias de cor (ex: `.color-primary`, `.bg-red`).
- **`_layout.scss`**: Controla o layout principal do site. Inclui a definição de `containers`, um sistema de `grid` de 12 colunas e um `mixin` para media queries que facilita a criação de layouts responsivos.
- **`_spacing.scss`**: Fornece um conjunto de classes utilitárias para definir `margins` e `paddings` de forma consistente, baseadas em uma escala de espaçamento pré-definida.
- **`_typography.scss`**: Gerencia toda a tipografia do projeto. Define `mixins` para tamanhos de fonte responsivos (h1, h2, p, etc.) e classes utilitárias de texto.

#### `style.css` e `style.css.map`

- **`style.css`**: O arquivo CSS final, gerado a partir da compilação de todos os arquivos `.scss`. É este arquivo que o `index.html` utiliza.
- **`style.css.map`**: Um sourcemap gerado pelo compilador SASS. Ele ajuda a depurar o código no navegador, mapeando o CSS compilado de volta para o código SASS original.

### `js/`

Este diretório é destinado a todos os arquivos JavaScript do projeto.

- **`svg-inject.min.js`**: Uma biblioteca JavaScript que permite injetar o conteúdo de arquivos SVG diretamente no DOM, facilitando a manipulação de seus estilos (como cores e traços) via CSS.

### `svg/`

Um diretório para armazenar todos os ícones e imagens no formato SVG que serão utilizados no projeto.

## Como Usar

1.  **Edite o `index.html`**: Adicione o conteúdo da sua página dentro da tag `<body>`.
2.  **Desenvolva com SASS**: Modifique os arquivos `.scss` no diretório `css/sass/` para estilizar seu site. Você precisará de um compilador SASS (como o Live Sass Compiler do VS Code ou a CLI do SASS) para gerar o `style.css` final.
3.  **Adicione JavaScript**: Coloque seus scripts no diretório `js/` e adicione a tag `<script>` correspondente no `index.html`.
4.  **Adicione SVGs**: Coloque seus arquivos `.svg` no diretório `svg/`.

Este projeto está pronto para ser expandido. Você pode adicionar mais arquivos SASS, scripts JS ou o que for necessário para o seu site.
