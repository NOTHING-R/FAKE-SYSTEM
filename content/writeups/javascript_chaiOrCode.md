+++
title = "javascript_chaiOrCode"
date = "2026-04-23"
author = "NOTHING-R"
+++
# Table of Contents
- [VAR LET AND CONST](#var-let-and-const-video-04)
- [DataTypes and ECMA](#datatypes-and-ecma-video-05)
  - [ECMA](#ecma)
  - [DataTypes](#datatypes)

# VAR LET AND CONST (video-04)
Modern js a sudhu matro `let` abong `const` use kora hoi karon. `var` er problem hocce var kno a scope kaj kore na. mane same name a akta varibale banale oi name a r kno varibale banano jai na 
```javascript
var hello = "name"
function vhurum(){
  var hello = "hi"
  console.log(hello)
}
console.log(hello)
```

```python
print("Hello")
```


# DataTypes and ECMA (video-05)
javascript a akta  syntex ace `use strict` aydar mane hocce js er j enginee ace oita js er ay code ta k new code er moto treate korb karon js ager theke onk besi mordern abong evolbe hoice. 
## ECMA 
`ECMA` hocce stander. Mane history er first er dike ak akta browser er system ak ak rokom cilo jar karone akta browser er jonno lekha code onno browser a kaj korto na. er pore `ECMA` ak jaigai hoye stander banai j code ay vabe e lekah hobe r browser gulo o ay code k ayvabe treate korbe...

## DataTypes
### NUMBER
number hocce full number jemon
```javascript
let age = 33
```
number er range hocce `2 to the power 53` jdi er theke boro number store korete hoi tahole `bigint`  use kora lage.....normaly to lage na kintu onk boro company jemon meta, redit ay sob a dorkar pore

### STRING
double othoba single qoute a ja ace sob string

```javascript
let name = "nothing"
```

### boolean
True othoba false 

### NULL
null hocce akta `standalone value` 

### UNDEFIEND

UNDEFIEND hocce jdi kno variable declear kore oita te kno value assign kora na hoi tahole

```javascript
let area; 
console.log(area) //Undefiend
```

### symbol
Symbol maily react type er jinis a use hoi ayta k `unique` dekhanor jonno use kroa hoi 

### OBJECT
object to data type j ta js er main data type 

## KIVABE DATA TYPE DEKHA JAI 
data type dekhar jonno 
```javascript
console.log(typeof "name")
console.log(typeof null)
console.log(typeof undifiend)
```
::RESULT::
string
object
undefined

inteview te ay quetion ta ase j null er data type ki? oitar ans hobe hocce object. Kintu undefined abr akta indivudual data type.

# DATA TYPE CONVERSTION CONFUSION (video-06)
CONVERSTION hocce akta dataType dia onno data type a convert kora string to number number to float float to number etc.
## akta kahini string to number er
```javascript
let age = "33"
console.log(typeof age)
let newAge = Number(age)
console.log(typeof newAge)
console.log(newAge)
```
::RESULT::
string
number
33

akhn jdi string er vitore kno charecter thake tkhn ki hobe? 
```javascript
let age = "33abc"
console.log(typeof age)
let newAge = Number(age)
console.log(typeof newAge)
console.log(newAge)
```
::RESULT::
string
number
NaN

`NaN` not a number mane ayda js er akta kahini j jdi charecter o theke tao nmbr a convert kore kintu oitar akta specila data type a convert kore ja hocce not a nmbr 

```javascript
let age = null
console.log(typeof age)
let newAge = Number(age)
console.log(typeof newAge)
console.log(newAge)
```
::RESULT::
object
number
0

null k number a convert korle hoi 0 r undefined k convert korle hoi NaN
## BOOLEAN CONVERSTION
1 = true
0 = fasle 
| True     | False |
| 1        | 0     |
| "string" | ""    |

# CONFIUSION BETWEEN STRING TO NUMBER CONVERSTION (video-07)
`Operation`  mane hocce +,-,*,/ ay sob  
```javascript
console.log(2+2)
console.log(2-2)
console.log(2/2)
console.log(2*2)
console.log(2**2)
console.log(2%2)

let value = 3
value = -value
console.log(value)
```

## kemon jeno ay code gulo 
```javascript
console.log(2 + 1 + "1")
//31
console.log("2" + 1 + 1) 
//211
```

```javascript
console.log(+true)
//1
console.log(+"")
//0
```

## ++ prefix a rakhle ki hoi r last a rakhle ki hoi 
[mdn docs](https:/*developer.mozilla.org*en-US*docs*Web*JavaScript*Reference*Operators*Increment)

# Comparison of datatypes in javascript (video-08)
```js
console.log(null > 0)
console.log(null == 0)
console.log(null >= 0)
--- Output
false
false
true
```
equalit == r Comparison alada vabe kaj kore Comparison <,>,!= same data type baniye nei ay jonno null 0 hoye jai r last a oita k `true` show kore 

## Strict check 
js a `==` data type check kore na jemon "1" == 1 true, jdio akta strirng r akta int....ay jonno equalit check er jonno sob smy `===` use kora hoi . Main kotha hocce == data type check kore na r === data type check kore Comparison kore 
```js
console.log("2" == 2)
console.log("2" === 2)
--- Output
true
false
```

#  Data types of javascript summary (video-09)
js er data type mainly 2 vag a vag kora. `premitive` r `Non-premetive`. premitive r Non-premetive hisab kora hoi hocce `kon vabe data k memory te rakha hoi abong access kora hoi oitar upore depend kore data type a ay dui vag a vag kora hoi`

## PREMITIVE
premitive a total 7 type er data type ace 

1. String  
String hocce normall "" er vitore ja ace ty 
2. Number 
3. BOOLEAN
4. NULL
null mane hocce kiccu na mane oita kno data type e na....null nijei alalda akta data type
5. undefined
undefined mane hocce akta variable declear kore oita te kno value dea hoi ni...ba variable ta te kno value nai 

