**Ответ: undefined.**
```js
var user = {
  firstName: "Василий",

  export: this // (*)
};

alert( user.export.firstName );
```
Объявление объекта само по себе не влияет на this. Никаких функций, которые могли бы повлиять на контекст, здесь нет.

Так как код находится вообще вне любых функций, то this в нём равен window (в браузере так всегда для кода вне функций, вне зависимости от use strict).

Получается, что в строке (*) мы имеем export: window, так что далее alert(user.export.firstName) выводит свойство window.firstName, которое не определено.

[task](https://github.com/y4t6/convert/blob/master/5_2.md)
