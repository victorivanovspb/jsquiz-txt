# Вопросы по JavaScript #3

**№1** Что будет результатом выполнения данного кода?

```
console.Log('Green');
```

- [x] TypeError
- [ ] null
- [ ] "Green"
- [ ] string 

TypeError: console.**Log** is not a function

---

**№2** Что будет выведено на консоль?

```
console.log(0 ? 0 : 1);
```

- [x] 1
- [ ] false
- [ ] true
- [ ] 0 

---

**№3** Что будет результатом выполнения следующего кода?

```
console.log(typeof typeof 2);
```

- [ ] undefined
- [ ] number
- [x] string
- [ ] object
- [ ] null    

---

**№4** Что будет выведено в результате?

console.log(null === null);

- [ ] false
- [ ] Возникнет ошибка
- [x] true
- [ ] null
- [ ] NaN

---
    
**№5** Что будет выведено после выполнения данного кода?

```
var numbers = Array(2,10);
numbers[numbers.length] = 0;
console.log(numbers.length);
```

- [ ] 0
- [x] 3
- [ ] 2
- [ ] Возникнет ошибка
- [ ] -1 

---
**№6** Что будет результатом выполнения следующего кода?

```
let user = {
    name: "Max",
    go: function() {
        return this.name;
    }
}

(user.go)();
```

- [ ] undefined
- [x] Возникнет ошибка
- [ ] Max

ReferenceError: can't access lexical declaration 'user' before initialization.  
Стоит разделить точкой с запятой объявление объекта и вызов метода. 

---
**№7** Что будет результатом выполнения следующего кода?

```
let user = {
    name: "Max",
    go: function() {
        return this.name;
    }
};

(user.go)();
```

- [ ] undefined
- [ ] Возникнет ошибка
- [x] Max

---
**№8** Что будет результатом выполнения следующего кода?

```
let user = {
    name: "Max",
    go: () => this.name
};

user.go();
```

- [x] undefined
- [ ] Возникнет ошибка
- [ ] Max

---

**№9** Что будет результатом выполнения следующего кода?

```
let user = {
    name: "Max",
    go: () => this.name
};
let obj = {
    name: "Alex",
};
user.go.call(obj);

```

- [ ] undefined
- [ ] Возникнет ошибка
- [x] ""
- [ ] Max
- [ ] Alex

---

**№10** Что будет результатом выполнения следующего кода?

```
let user = {
    name: "Max",
    go: function () {
        return this.name;
    }
};

let obj = {
    name: "Alex",
};

user.go.call(obj);
```

- [ ] undefined
- [ ] Возникнет ошибка
- [x] ""
- [ ] Max
- [ ] Alex

---

**№11**
```
var a = {
    name: 'a',
    foo: function () {
        console.log(this.name);
    }
};

a.foo();
```

- [ ] Возникнет ошибка
- [ ] undefined
- [x] "a"
- [ ] ""

---

**№12**
```
var a = {
    name: 'a',
    foo: function () {
        console.log(this.name);
    }
};

var bar = a.foo;
bar();
```

- [ ] Возникнет ошибка
- [x] undefined
- [ ] "a"
- [ ] ""

---

**№13**
```
var a = {
    name: 'a',
    foo: function () {
        console.log(this.name);
    }
};

var b = {
    name: 'b'
};

b.foo = a.foo;
b.foo();
```

- [ ] Возникнет ошибка
- [ ] undefined
- [ ] "a"
- [x] "b"
- [ ] ""

---

**№14**
```
var a = {
    name: 'a',
    foo: function () {
        console.log(this.name);
    }
};

var bar = a.foo;
var c = {
    name: 'c'
};
bar.call(c);
```

- [ ] Возникнет ошибка
- [ ] undefined
- [ ] "a"
- [x] "c"
- [ ] ""

---

...

a.foo.apply(b); // 'b'  
a.foo.bind(b).call(c); // 'b'  
a.foo.bind(b).bind(c)(); // 'b'  
