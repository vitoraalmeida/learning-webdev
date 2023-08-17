## Separação de arquivos css:

```
styles
    components -> cada componente da página num arquivo
        header.css
        footer.css
        hero.css
    global.css -> resets
    util.css   -> classes utilitárias (ex.: .container .btn)
index.html
```

No index.html adicionamos primeiro o arquivo globals.css, depois os componentes e por ultimo a utils, pela ordem de especificidade

No global.css colocamos os resets

No utils.css colocamos uma classe .container que será adicionada em cada componente, além disso colocamos as media queries para mobile-first ou desktop-first

```
/*mobile first */
/* xs */
@media (min-width: 475px) {
}

/* sm */
@media (min-width: 640px) {
}

/* md */
@media (min-width: 768px) {
}

/* lg */
@media (min-width: 1024px) {
}

/* xl */
@media (min-width: 1280px) {
}

/* 2xl */
@media (min-width: 1536px) {
}

/* desktop first */
/* 2xl */
@media (max-width: 1536px) {
}

/* xl */
@media (max-width: 1280px) {
}

/* lg */
@media (max-width: 1024px) {
}

/* md */
@media (max-width: 768px) {
}

/* sm */
@media (max-width: 640px) {
}

/* xs */
@media (max-width: 475px) {
}
```
