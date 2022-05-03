## Converting a string to numbers in js 

* You can convert any data type to a number by adding a + or – sign before the element to be converted

````
let x = '5'; let x = 'Mujahed'; let x = undefined; let x = true; let x = null;

console.log(+x || +'5')// 
عند وضع (+) أو (-) أمام أي عنصر
 string 
 راح يعتبره كرقم 
 console.log(+'10'++'10') // 20
 console.log(+'Mujahed') // NaN(not a number)
console.log(+true) //1
console.log(+false) //0
console.log(+undefined) //NaN(not a number)
console.log(+null) //0
````
* Js can be converted from string to number automatically  using by calculate operations without plus
 
 لغة جافا سكربت بإمكانها تحويل النصوص الى أرقام بشكل تلقائي من خلال العمليات الحسابية بإستثناء علامة الجمع 
 ```
 console.log('5'+'5') //'55'
  console.log('10'-'6') //4
  console.log('10'*'6') //60
  console.log('10'/'5') //2
  console.log('2'**'2') //4(**الرقم الاول أس الرقم الثاني)
 ```