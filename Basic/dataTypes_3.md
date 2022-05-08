# DataTypes in Js

- Datatypes in general

1. Primitive
1. Non-Primitive

## I need to do with data in js

1. Send data.
1. Receive data.
1. Data manipulation.

## Pirmitive DataTypes

1. String( ' ' || " " )
1. Number( 10, 10.25, 0.251 )
1. Boolean ( true || false )
1. null (nothing (typeof ==object))
1. undefined(not found)

- To determine the type of data it used

```
console.log(typeof variable)
```

----
## Ways to declare variable

1. var

```
var x=10;
-----
var y;
y=50;
y=70;
-----
var r=6;
var r=8; // Re-declaration
All these ways correct in var 
```
2 . let
````
let x;
x=10;
x=50;
-----
let x=10;
-----
let x=10
let x=50
error, not correct I can't do Re-declaration do this way (let again)   
correct(x=50)
````

3. const 

`````
const x=50;
just this a way is correct in const 

-----
const x;
x=50 
or 
const x=30;
x=40;
or
 const x=10;
const x=20;
All these a ways  mistake in const 
because when we declare a variable by const
that's means I give this variable a constant value I can't re-declaration (قيمة ثابتة لا يمكن اعادة اعطائها قيمة أخرى أو تبديلها ) 
`````
