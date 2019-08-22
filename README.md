### snow <https://jumpzilla.github.io/snow/>
***
По ссылкам пока переходит только через опцию "Открыть в новой вкладке". Проблема наблюдается не только у меня, и возникает из-за этого js-скпипта "slow scroll", консоль ругается на пятую строчку, при этом сам скрипт отрабатывает.
```js
// slow scroll
1 $(document).ready(function(){
2   $("#menu").on("click","a", function (event) {
3     event.preventDefault();
4     var id  = $(this).attr('href'),
5     top = $(id).offset().top;
6     $('body,html').animate({scrollTop: top}, 1500);
7   });
8 });
```
***
