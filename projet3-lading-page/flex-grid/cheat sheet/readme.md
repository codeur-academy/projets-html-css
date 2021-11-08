# Cheat sheet Flex

## HTML

```html
<body class="container">
    <main class="row">
        <aside class="col-xs-12 col-md-3 col-lg-2">
        </aside>
        <article class="col-xs-12 col-md-6 col-lg-8">
        </article>
    </main>
    <footer class="row">
    </footer>
</body>
```


# Cheat sheet Flex - Grid

## index.html

```html
<body class="container">
    <main class="row">
        <aside class="col-xs-12 col-md-3 col-lg-2">
        </aside>
        <article class="col-xs-12 col-md-6 col-lg-8">
        </article>
    </main>
    <footer class="row">
    </footer>
</body>
```


## style.css

```css
header nav ul  {
    display: flex;
    list-style: none;
}
header nav ul li{
    flex : 0 0 100px;
}
```


## flex-grid.css

```css
.container {
}

.row {
  box-sizing: border-box;
  display: flex;
  flex: 0 1 auto;
  flex-direction: row;
  flex-wrap: wrap;
}

/* xs =  x-small */
.col-xs,
.col-xs-1,
.col-xs-2,
.col-xs-3 {
  box-sizing: border-box;
  flex: 0 0 auto;
  padding-right: 0.5rem;
  padding-left: 0.5rem;
}

.col-xs {
  flex-grow: 1;
  flex-basis: 0;
  max-width: 100%;
}

.col-xs-1 {
  flex-basis: 8.33333333%;
  max-width: 8.33333333%;
}


/* Répétition en sm */

/* sm : small screens */
@media only screen and (min-width: 48em) {
  .container {
    width: 49rem;
  }
 }

/* md */
@media only screen and (min-width: 64em) {
  .container {
    width: 65rem;
  }
}

/* lg */
@media only screen and (min-width: 75em) {
  .container {
    width: 76rem;
  }


}

```