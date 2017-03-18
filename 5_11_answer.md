```js
function Accumulator(startingValue) {
  this.value = startingValue;

  this.read = function() {
    this.value += +prompt('Сколько добавлять будем?', 0);
  };

}

var accumulator = new Accumulator(1);
accumulator.read();
accumulator.read();
alert( accumulator.value );
```

[task](https://github.com/y4t6/convert/blob/master/5_11.md)
