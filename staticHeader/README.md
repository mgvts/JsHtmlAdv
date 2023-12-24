some page examples my view of correct static header webbpage

It's made without `position:fixed` or `position:sticky`

I make it with this one
```html
<div class="page">
  <header class="header">
    ...
  </header>
  <div class="content">
    ...
  </div>
  <footer  class="footer">
    ...
  </footer>
</div>
```


```css
.page {
  display: flex;
  flex-direction: column;
  height: 100vh;
  overflow: hidden;
}
.content {
  height: 100%;
  overflow-y: auto;
}
.header {
  top:0;
}
.footer {
  bottom: 0;
}
```

because I don't use `fixed/stciky` can easily add some popup
without any refactor of this code
