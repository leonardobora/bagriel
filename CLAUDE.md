# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Sobre o projeto

Fan site cursed (inside joke) do **Bagriel** (Gabriel Busch Gomes de Sá). Single-file HTML, sem build, sem framework, sem dependências. Estética proposital: WordArt do Word 97, ASCII art, cores berrantes, `<marquee>`, hit counter — visual early-2000s GeoCities.

Tudo vive em `index.html`. CSS é inline (`<style>` no `<head>`). Não há JS.

## Como rodar / desenvolver

- **Local:** abrir `index.html` direto no navegador (file://) ou servir com `python -m http.server` no diretório raiz.
- **Build:** não tem. Edição é direto no HTML.
- **Deploy:** GitHub Pages, branch `main`, pasta raiz. Push pra `main` já publica.

## Convenções de conteúdo (importante pra manter o tom)

- É **BAGRIEL**, nunca "Gabriel" no copy do site (exceto onde explicitamente esclarecendo o nome real). O typo é o ponto.
- Tom: cursed-affetuoso, exagerado, fan-site não-oficial-mas-bem-oficial. Não suavizar.
- Fontes externas: Google Fonts (`Press Start 2P`, `VT323`). Já carregadas via `@import` no CSS.
- Seções existentes seguem o padrão `<section class="secao">` com `<h2>` em ASCII-ornamentado (`~ * X * ~`, `:: X ::`, `>> X <<`). Manter o padrão ao adicionar seções.
- Classes utilitárias já definidas: `.wordart` (+ `.rainbow`, `.curvado`), `.fato`, `.moldura`, `.botao-90s`, `.glow`, `.hitcounter`. Reusar antes de criar novas.

## Estrutura de uma seção típica

```html
<section class="secao">
  <h2>:: TÍTULO ::</h2>
  <div class="fato"><span class="label">FATO N →</span> ...</div>
</section>
```

`<div class="moldura">` envolve ASCII art com legenda estilo polaroid.
