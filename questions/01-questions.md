
## Useful links 
- http://perfectionkills.com/javascript-quiz/
- learn.javascript.ru/quiz

## Questions
№1

```
(function(){
    return typeof arguments;
})();
```

- [ ] "array"
- [x] "object"  
- [ ] "arguments"
- [ ] "undefined"

---
№2

```
var f = function g(){ return 23; };
typeof g();
```

- [ ] "number"
- [ ] "undefined"
- [ ] "function"
- [x] Error

---
3

```
(function(x){
    delete x;
    return x;
})(1);
```

- [+] 1
- [ ] null
- [ ] undefined
- [ ] Error


-------------------------------------------------------------------------------
Вопрос 4

var y = 1, x = y = typeof x;
x;

- [ ] 1
- [ ] "number"
- [ ] undefined
- [+] "undefined"

---
Вопрос 5

(function f(f){
    return typeof f();
})(function(){ return 1; });

- [+] "number"
- [ ] "undefined"
- [ ] "function"
- [ ] Error

---
Вопрос 6

var foo = {
    bar: function() { return this.baz; },
    baz: 1
};
(function(){
    return typeof arguments[0]();
})(foo.bar);

- [+] "undefined"
- [ ] "object"
- [ ] "number"
- [ ] "function"

---
№7

```
var foo = {
    bar: function(){ return this.baz; },
    baz: 1
}
typeof (f = foo.bar)();
```

- [+] "undefined"
- [ ] "object"
- [ ] "number"
- [ ] "function"

---
№8

```
var f = (function f(){ return "1"; }, function g(){ return 2; })();
typeof f;
```

- [ ] "string"
- [x] "number"
- [ ] "function"
- [ ] "undefined"

---
№9

```
var x = 1;
if (function f(){}) {
    x += typeof f;
}
x;
```

- [ ] 1
- [ ] "1function"
- [x] "1undefined"
- [ ] NaN

---
№10

```
var x = [typeof x, typeof y][1];
typeof typeof x;
```

- [ ] "number"
- [x] "string"
- [ ] "undefined"
- [ ] "object"

---
№11

```
(function(foo){
    return typeof foo.bar;
})({ foo: { bar: 1 } });
```

- [x] "undefined"
- [ ] "object"
- [ ] "number"
- [ ] Error

---
№12

```
(function f(){
    function f(){ return 1; }
    return f();
    function f(){ return 2; }
})();
```

- [ ] 1
- [x] 2
- [ ] Error (e.g. "Too much recursion")
- [ ] undefined

---
№13

```
function f(){ return f; }
new f() instanceof f;
```

- [ ] true
- [x] false

---
№14

```
with (function(x, undefined){}) length;
```

- [ ] 1
- [x] 2
- [ ] undefined
- [ ] Error

В режиме `'use strict'` конструкция with не работает (признана устаревшей).
Function.length возвращает кол-во ожидаемых функцией аргументов.

---
№15. Чему равен результат вызова в этом примере?

```
function f() {
    let a = 5;
    return new Function('b', 'return a + b');
}
alert( f()(1) );
```

- [ ] 1
- [ ] 6
- [ ] undefined
- [ ] NaN
- [x] Будет ошибка.


