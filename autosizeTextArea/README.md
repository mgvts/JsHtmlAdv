#some example about textarea with autoheight

here some code about
```html
<textarea class="auto-height">
  put ur text here and enjoy it
</textarea>

```
```css
.auto-height {
  overflow-y: hidden;
  resize: none;
}
```
```javascript
const autosize = document.querySelector(".auto-height")
autosize.addEventListener('input', () => {
    autosize.style.height = 'auto';
    autosize.style.height = (autosize.scrollHeight) + 'px';
})
```