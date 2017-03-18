Решение состоит в том, чтобы каждый раз возвращать текущий объект. Это делается добавлением return this в конце каждого метода:
```js
var ladder = {
  step: 0,
  up: function() {
    this.step++;
    return this;
  },
  down: function() {
    this.step--;
    return this;
  },
  showStep: function() {
    alert( this.step );
    return this;
  }
}

ladder.up().up().down().up().down().showStep(); // 1
```
[task](https://github.com/y4t6/convert/blob/master/2_1.md)
