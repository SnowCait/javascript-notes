# JavaScript

## 各ブラウザのサポート状況
- [Can I use](https://caniuse.com/)

## フレームワーク
軽 < Vue < Angular < React < 重

## Log
- `console.log()`
- `console.warn()`
- `console.error()`

## Form
- https://qiita.com/bami3/items/102d0748ed99658953c5
```javascript
document.querySelectorAll('.ajax-form').forEach((form) => {
  form.addEventListener('submit', (event) => {
    console.log('Request Ajax.', form);
    event.preventDefault();
    const $form = $(form);
    $.ajax({
      method: form.method,
      url: form.action,
      data: $form.serialize(),
      dataType: 'text'
    })
    .then((data) => {
      console.log('Success Ajax.', data);
    })
    .catch((error) => {
      console.log('Failed Ajax.', error);
    });
  });
});
```

## IDE
### IntelliJ
- [`<script>` のインデントをしない](https://intellij-support.jetbrains.com/hc/en-us/community/posts/360000000110-Code-Style-Javascript-indent-problems)

