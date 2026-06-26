# Snitap Patins — CSS Animations & Transitions Study Project

Landing page fictícia de uma marca de patins, criada para estudar e praticar conceitos de **CSS Transitions** e **CSS Animations**.

## Preview do design

[Visualizar protótipo no Figma](https://www.figma.com/proto/tkBX0Dkz5Ml5EQw6Pq0TEz/LP-de-patins-animada--Community-?node-id=3-811&t=Zw6gQHaNXrtOUqTl-1&scaling=min-zoom&content-scaling=fixed&page-id=3%3A376&starting-point-node-id=3%3A811)

## Sobre o projeto

A página simula o site de uma marca chamada **Snitap** e foi construída inteiramente com HTML e CSS puros — sem JavaScript. O foco está nas técnicas de animação e transição do CSS aplicadas em cenários reais de UI.

## Tecnologias utilizadas

- **HTML5** — estrutura semântica da página
- **CSS3** — estilização, animações e transições
  - Custom Properties (variáveis CSS)
  - CSS Nesting
  - Flexbox e CSS Grid
  - `@keyframes`
  - `animation-timeline: view()` (Scroll-driven Animations)
  - `@media` queries para responsividade
- **Google Fonts** — fontes Inter, Montserrat e Syne

## Conceitos de CSS praticados

| Seção | Técnica |
|---|---|
| **Header** | `transition: transform` — rotação dos ícones ao hover |
| **Hero** | `@keyframes slideUp` — troca cíclica de palavras com efeito bounce; `@keyframes slideIn` — entrada da imagem do produto deslizando da direita; `animation-fill-mode`, `animation-delay` |
| **Banner** | `@keyframes rolling` — scroll infinito de imagens; `@keyframes bg-gradient` — gradiente de fundo animado com `background-size` e `background-position` |
| **Galeria** | `animation-timeline: view()` — aparecimento das fotos conforme o scroll (Scroll-driven Animations); `transition: scale` e `transition: transform` — efeito de zoom e overlay ao hover |
| **Footer** | `transition: transform` no pseudo-elemento `::after` — underline animado nos links; `transition: transform` no pseudo-elemento `::before` — background circular nos ícones sociais |

## Estrutura do projeto

```
animations-project/
├── assets/
│   ├── icons/          # SVGs: logo, ícones de UI e redes sociais
│   └── images/         # Imagens da galeria e do produto
├── styles/
│   ├── index.css       # Ponto de entrada — importa todos os demais arquivos CSS
│   ├── global.css      # Reset, variáveis CSS e tipografia base
│   ├── header.css      # Estilos e animações do cabeçalho
│   ├── hero.css        # Estilos e animações da seção hero
│   ├── banner.css      # Estilos e animações do banner rolante
│   ├── gallery.css     # Estilos e animações da galeria de fotos
│   └── footer.css      # Estilos e animações do rodapé
├── banner.svg          # SVG do banner rolante
└── index.html          # Página principal
```

## Como rodar o projeto

Este projeto usa apenas HTML e CSS estáticos. A forma recomendada é utilizar o plugin **Live Server** do VS Code:

1. Abra a pasta do projeto no **VS Code**
2. Instale a extensão [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) (caso ainda não tenha)
3. Clique com o botão direito no arquivo `index.html` e selecione **"Open with Live Server"**
4. O navegador abrirá automaticamente em `http://127.0.0.1:5500`

> Alternativamente, basta abrir o arquivo `index.html` diretamente no navegador, mas o Live Server oferece recarga automática ao salvar alterações.

## Responsividade

O layout é responsivo e se adapta a telas menores (mobile-first). O breakpoint principal está em `80rem` (1280px), onde o layout passa de coluna única para colunas lado a lado.
