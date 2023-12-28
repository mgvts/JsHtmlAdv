some page examples my view of correct static header webbpage

I make it with this one `HeaderPage.html`
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

same logic with `position:fixed`,
but to updating `height` (adding `margin`)
we need some js code

```javascript
const header = document.querySelector('.header')
const footer = document.querySelector('.footer')
const content = document.querySelector('.content')

const unpdateMargin = () => {
    content.style.marginTop = header.clientHeight + 'px'
    content.style.marginBottom = footer.clientHeight + 'px'
}
```
