# Loja de Patins | Snitap

Landing page estática de uma loja fictícia de patins, com foco em apresentação visual, animações em CSS e uma galeria de fotos com identidade jovem e vibrante.

## Página publicada

https://gabrielsants7.github.io/Loja-de-Patins/

## Visão geral

O projeto foi construído com HTML e CSS puro, sem dependências de framework ou etapa de build. A página apresenta:

- cabeçalho com logo e ícone de carrinho;
- seção hero com chamada principal, animação de palavras e CTAs;
- faixa horizontal animada em destaque;
- galeria de fotos com efeito de entrada e hover;
- rodapé com navegação institucional e links sociais.

## Tecnologias utilizadas

- HTML5
- CSS3
- Google Fonts

## Estrutura do projeto

```text
Loja-de-Patins/
|-- assets/
|   |-- banner.svg
|   |-- person.png
|   |-- hero/
|   |-- icons/
|   `-- images/
|-- styles/
|   |-- index.css
|   |-- global.css
|   |-- header.css
|   |-- hero.css
|   |-- banner.css
|   |-- gallery.css
|   `-- footer.css
|-- index.html
`-- README.md
```

## Como executar localmente

Como este é um projeto estático, basta servir os arquivos em um servidor local simples.

### Opção 1: Live Server no VS Code

1. Abra a pasta do projeto no VS Code.
2. Instale a extensão `Live Server`, se necessário.
3. Clique com o botão direito em `index.html`.
4. Selecione `Open with Live Server`.

### Opção 2: servidor HTTP simples

Se você tiver Python instalado:

```bash
python -m http.server 5500
```

Depois abra no navegador:

```text
http://localhost:5500
```

## Organização dos estilos

Os estilos foram divididos por responsabilidade:

- `styles/index.css`: ponto central de importação dos demais arquivos CSS.
- `styles/global.css`: reset, variáveis, tipografia e estilos globais.
- `styles/header.css`: cabeçalho e contador do carrinho.
- `styles/hero.css`: seção principal, botões e animações da hero.
- `styles/banner.css`: faixa rolante com gradiente animado.
- `styles/gallery.css`: grid da galeria, animações de entrada e overlay.
- `styles/footer.css`: rodapé, navegação e ícones sociais.

## Destaques visuais

- Palavras animadas no título principal usando `@keyframes`.
- Entrada dos elementos da hero com transições e deslocamento horizontal.
- Banner com rolagem contínua e gradiente animado.
- Galeria com efeito de revelação ao entrar na viewport.
- Interações de hover em imagens, links e ícones.

## Personalização

Você pode adaptar rapidamente o projeto alterando:

- textos e links em `index.html`;
- cores em `:root` dentro de `styles/global.css`;
- imagens da hero, galeria e ícones na pasta `assets/`;
- animações e timings nos arquivos CSS por seção.

## Observações técnicas

- O projeto depende de fontes carregadas via Google Fonts.
- Alguns recursos usados no CSS, como aninhamento e `animation-timeline`, podem ter suporte diferente dependendo do navegador e da versão utilizada.
- Se houver problema com acentuação em alguns textos, confirme se os arquivos estão salvos em UTF-8.
- Há uma regra `zoom: .3` em `styles/global.css`; ela impacta diretamente a escala geral da interface e pode exigir ajuste para diferentes contextos de exibição.

## Próximos passos sugeridos

- melhorar a responsividade para diferentes tamanhos de tela;
- adicionar links reais para CTA, navegação e redes sociais;
- revisar acessibilidade de `alt`, contraste e navegação por teclado;
- incluir um favicon e metadados sociais;
- corrigir e padronizar textos com acentuação, se necessário.
