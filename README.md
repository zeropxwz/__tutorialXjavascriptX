# Переменные

Для объявления переменных и констант используются ключевые слова __var__, __let__ и __const__

__var__ и __let__ объявляют переменные, а __const__ постоянные значения

## Декларация и инициализация 

Переменные или константы можно сначала объявить, а потом присвоить значение:

```ts
// первый вариант
var a: number
var b: number
var c: number | null

    a = 10
    b = 2
    c = null

// второй вариант
var 
    a: number, b: number, c: number
   
    a = 10
    b = 2
    c = null
  
// третий вариант
var 
    a: number,
    b: number,
    c: number | null
    
    a = 10
    b = 20
    c = null
```

Но можно присвоить значение и сразу при объявлении:

```ts
// первый вариант
var a: number        = 10
var b: number        = 2
var c: number | null = null

// второй вариант
var 
    a: number = 10, b: number = 2, c: number | null = null          

// третий вариант
var 
    a: number        = 10
    b: number        = 2
    c: number | null = null 
```

Также, если не включен "strict mode" переменную можно объявлять просто как `a = 10`, что не рекомендуется

## разница между __var__ и __let__

И __var__ и __let__ объяляют переменные, но между ними есть существенное различие

### область видимости 

```ts
//
//
// описание про область видимости
```

Кроме того есть и другие различия:  

__1.__  

__var__ можно объявлять несколько раз, что может привести к случайному переназначению и багам:

```ts
var x = 10

// code pipe
// code pipe
// code pipe

var x = 2
```

в то время, как __let__ в таком случае выбросит ошибку:

```ts
let x = 10

// code pipe
// code pipe
// code pipe

let x = 2 // SyntaxError: Identifier 'x' has already been declared
```

__2.__  

__var__ можно хостить:

```ts
x = 2
console.log(x) // выведет 2

var x
```

а __let__ нет:

```ts
x = 2
console.log(x) // ReferenceError: Cannot access 'x' before initialization

let x
```

## __const__

__const__ во всем ведет себя подобно __let__ за исключением одного - присвоенное значение является константным и его нельзя переназначить.

```ts
const x: number = 10

      x = 2 // Cannot assign to 'x' because it is a constant
``` 





















    
