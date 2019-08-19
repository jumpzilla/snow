### snow <https://jumpzilla.github.io/snow/>
***
По ссылкам пока переходит только через опцию "Открыть в новой вкладке". Проблема наблюдается не только у меня, и возникает из-за js-кода на пятой строчке 
```js
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
