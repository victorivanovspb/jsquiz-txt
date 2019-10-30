# Вопросы по JavaScript #2

**№16** Что будет выведено в консоль после выполнения данного кода?

```
var a = { b : "c" };
console.log(typeof a);
```

- [ ] undefined
- [ ] false
- [ ] "c"
- [ ] string
- [x] object 

---

**№17** Каков будет результат выполнения следующего кода?

```
var a = new Array(5,50);
var b = new Array(5,50);
console.log(a == b);
```

- [ ] true
- [x] false
- [ ] null
- [ ] undefined 

---

**№18** Является ли JavaScript регистрозависимым?

- [ ] Нет
- [x] Да

---

**№19** Что будет выведено в консоль после выполнения данного кода?

```
console.log(typeof null);
```

- [x] object
- [ ] true
- [ ] null
- [ ] false
- [ ] undefined 

---

**№20** Каков будет результат выполнения данного кода?

```
var digitsArray = [1,2,3];
Array.prototype.each = function() {}

var result = '';

for (var digit in digitsArray) {
    result += digit;
}

console.log(result);
```

- [ ] 123each
- [ ] 123
- [x] 012each
- [ ] 123function
- [ ] 012
- [ ] 012function

---

**№21** Что будет выведено?

```
var digitArray = [];
digitArray[5] = 10;

console.log(digitArray.length);
```

- [x] 6
- [ ] 5
- [ ] Упадёт ошибка
- [ ] 1 

---

**№22** Что будет выведено на консоль?

```
console.log(0.7 + 0.2);
```

- [ ] 0.9
- [ ] "0.9"
- [ ] 0,9
- [x] Другое
- [ ] "0,9"

---

**№23** Каков будет результат выполнения данного кода?

```
console.log(11111111111111111 === 11111111111111113);
```

- [ ] undefined
- [ ] NaN
- [x] true
- [ ] false

---

**№24** Что будет выведено после выполнения данного кода?

```
console.log(false + false);
```

- [ ] false
- [ ] undefined
- [ ] NaN
- [x] 0
- [ ] "falsefalse"
- [ ] 1 

---

**№25** Что будет выведено в результате?

```
var userArray = new Array(3);
console.log(userArray.toString());
```

- [ ] undefined
- [x] ,,
- [ ] []
- [ ] ,

---

**№26** Что будет выведено на консоль?

```
console.log(1 + '2' + 3);
```

- [ ] 5
- [ ] 6
- [x] 123
- [ ] 15 

---

**№27** Что будет являться результатом выполнения?

```
var message = 'H';
console.log(message.concat('n'));
```

- [x] Hn
- [ ] 0
- [ ] undefined
- [ ] null
- [ ] false 

---

**№28** Что будет являться результатом выполнения команды?

```
console.log(new String('Yellow') === 'Yellow');
```

- [ ] true
- [x] false
- [ ] 1
- [ ] 0
- [ ] undefined 

---

**№29** Что будет выведено?

```
console.log(NaN == NaN || NaN === NaN);
```

- [x] false
- [ ] undefined
- [ ] null
- [ ] true 

---

**№30** Что будет выведено в результате?

```
console.log(Math.min(null,200));
```

- [ ] 1
- [ ] 200
- [x] 0
- [ ] NaN
- [ ] null
- [ ] object 
