# JavaScript turorial

## Переменные 

Для объявления переменных и констант используются ключевые слова __var__, __let__ и __const__

__var__ и __let__ - это переменные  
__const__         - константное значние  

### Декларация и инициализация 

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






















    
