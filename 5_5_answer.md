```js
var calculator = {
  sum: function() {
    return this.a + this.b;
  },

  mul: function() {
    return this.a * this.b;
  },

  read: function() {
    this.a = +prompt('a?', 0);
    this.b = +prompt('b?', 0);
  }
}

calculator.read();
alert( calculator.sum() );
alert( calculator.mul() );
```
[task](https://github.com/y4t6/convert/blob/master/5_5.md)
