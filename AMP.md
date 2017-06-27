# AMP PROJECT

# Styles
Every amp page can only have a single embedded stylesheet
- Não pode referenciar nenhum stylesheet externa (com excessão das custom fonts)
- Inline styles attributes NÃO são permitidos

Todos os Styles devem ficar dentro a tag head do documento.

> **NOTA -**  AMP components vem com default styles

## Desabilitando styles
Os seguintes estilos não são permitidos em páginas AMP

Banned Style | Description
--- | ---
Inline style attributes | Todos os styles devem ser definidos no \<head> da página dentro do `<style amp-custom>`.
`!important` | Não é permitido seu uso. Isto é um requerimento necessário para abilitar AMP para forçar suas regras de tamanhos dos elementos.
\<link rel="stylesheet"> | Desabilitado exceto as custom fonts
`-amp-` class e `i-amp-` tag names | Não pode ser utilizadas. Estas são reservados para uso interno pelo AMP runtime.
`behavior`, `-moz-`, `binding` | Estas propriedades não são permitidas por rasões de segurança
`filter` | Listado por preocupações com a performance

## Custom fonts
AMP pages can’t include external stylesheets, with the exception of custom fonts. You can embed custom fonts into your page in two ways:

1. Through a <link> tag (white-listed font providers only)
2. Via @font-face (no restrictions, all fonts allowed)

## Layout & Media queries
AMP supports both media queries & element queries, plus comes with a powerful, built-in way to control the layout of individual elements. The layout attribute makes working with and creating fully responsive design much easier than if you'd use CSS alone.

### Responsive images, made easy
Create responsive images by specify the `width` and `height`, setting layout to `responsive`, and indicating with `srcset` which image asset to use based on varying screen sizes:

```html
<amp-img
  src="imgs/anitta.jpg"
  srcset="imgs/wide.jpg 640w,
          imgs/narrow.jpg 320w"
  width="1698"
  height="2911"
  layout="responsive"
  alt="an image">
</amp-img>
```

## GROW.io
Parecido com jekyll [sito to grow.io](http://grow.io/start/)


