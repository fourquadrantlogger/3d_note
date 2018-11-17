# ES6 语法

+ let 块级作用域
```
for (let i = 0; i < 10; i++) {
  // ...
}

console.log(i);
// ReferenceError: i is not defined
```
+ 块级作用域
```
{{}}
```
+ 数组
```
let [a, b, c] = [1, 2, 3];
```
+ 解构
```
const [a, b, c, d, e] = 'hello';
a // "h"
b // "e"
c // "l"
d // "l"
e // "o"
```
+ =>
```

[[1, 2], [3, 4]].map(([a, b]) => a + b);
// [ 3, 7 ]

[1, undefined, 3].map((x = 'yes') => x);
// [ 1, 'yes', 3 ]
```

+ 只要有可能导致解构的歧义，就不得使用圆括号

## 基本数据类型

ES6 引入了一种新的原始数据类型Symbol，表示独一无二的值。它是 JavaScript 语言的第七种数据类型，前六种是：undefined、null、布尔值（Boolean）、字符串（String）、数值（Number）、对象（Object）