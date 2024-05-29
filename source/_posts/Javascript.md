---
title: Javascript
date: 2024-05-29 16:38:27
tags:
- JS
- Frontend

---


## 🏅 [數字處理](https://www.w3school.com.cn/js/js_number_methods.asp)

### 四捨五入語法

```JavaScript
number.toFixed(digits)
```

| 參數 | 描述 |
| -------- | -------- |
| **digits**     | 可選小數位數，0~20之間的值(包含0和20)，默認為0(無小數)   |

### 字串轉數字

```JavaScript
Number(object)
```

| 參數 | 描述 |
| -------- | -------- |
| **object**     | JacaScript對象，若未提供該參數，則返回0；若值無法轉為數字，則返回NaN   |

### 餘數運算子

```JavaScript
x % y
```

```JavaScript
console.log(1%4) // 1
console.log(6%2) // 0
```

</br>

## 🏅 [字串設計](https://www.w3school.com.cn/js/js_string_methods.asp)

### 字串長度計算

```JavaScript
str.length
```

```JavaScript
var str = 'hello world';
str.length // 11

var str = '你好';
str.length // 2
```

### 英文強制小寫

```JavaScript
str.toLowerCase()
```

### 去除段落兩端空白

```JavaScript
string.trim()
```

```JavaScript
// input 輸入
trimString(" aa@gmail.com  ")

// output 輸出
"aa@gmail.com"
```

### 字串轉陣列

```JavaScript
txt.split(",");    // 用逗號分隔
txt.split(" ");    // 用空格分隔
txt.split("|");    // 用豎線分隔
```

```JavaScript
// input 輸入
splitString("black,red,white")

// output 輸出
["black","red","white"]
```

### 切割字串

```JavaScript
string.slice(start, end) 
```

| 參數 | 描述 |
| -------- | -------- |
| **start**| 可為負數，從字串結尾開始計數   |
| **end**| 可省略，將裁剪剩餘字串   |

```JavaScript
string.substring(start, end)
```

| 參數 | 描述 |
| -------- | -------- |
| **start**| 不可為負數   |
| **end**| 可省略，將裁剪剩餘字串   |

```JavaScript
string.substr(start, length)
```

| 參數 | 描述 |
| -------- | -------- |
| **start**| 可為負數，從字串結尾開始計數   |
| **lenfth**| 可省略，將裁剪剩餘字串   |

</br>

## 🏅 [運算式與運算子](https://developer.mozilla.org/zh-TW/docs/Web/JavaScript/Guide/Expressions_and_operators)

### 比較運算子

| 描述                            | 運算子 | 描述   |    運算子 |
| ----------------------------------- |:--------:| ----------- | --- |
| Equality        |   `==`   | Strict Equality |  `===` |
| Inequality      |   `!=`   | Strict Inequality |`!==` |
|Greater than|  `>`   | Greater than or equal      |  `>=`     |
| Less than     |   `<`      | Less than or equal        |  `<=`   |

### 邏輯運算子

>通常被用於布林(邏輯)值

| Operator | Usage | Description |
| -------- | -------- | -------- |
| Logical AND     | `運算式1 && 運算式2`   |兩個運算元都是 True 時才會回傳 True，否則回傳 false|
| Logical OR     | `運算式1｜｜運算式2`  | 兩個運算元有任一個是 True 時就會回傳 True，否則回傳 false   |
| Logical NOT    | `!運算式`   | 單一個運算元能被轉換成 True 時，回傳false ， 不然回傳 true     |

### 型別判斷

```JavaScript
typeof (運算元)
```

```JavaScript
// input 輸入
checkType(3.33)
checkType("Hello")
checkType(true)
checkType([1,2,3])

// output 輸出
"number"
"string"
"boolean"
"object"
```

</br>

## 🏅 If 流程判斷

### if/else 條件判斷

|  if / else          |           描述           |  if / else                |                描述                |
| --------------------------------------- |--------------------------------------------| --------------------------------------------- |------------------------------------------------------|
| `if…`          |        判斷式 : A        | `if… else…`        |      二分法判斷式 : A 或非 A       |
| `if… else if…` |  判斷兩種情況 : A 或 B   | `if… else if… else…`  | 三分法判斷式 : A 或 B 或「非A非B」 |
