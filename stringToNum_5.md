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
 ## Other ways to change the string to Numbers
   ````
   1. using by function called Number()=> any data inside ()convert to number 

   console.log(Number("4"))//4 (number) 
   يقوم بتحويل أي نص له قيمة رقمية إلى رقم 
   به عيب انه لا يستطيع تحويل الى رقم إذا اتى بعد الرقم نص 

  console.log(Number("4 mujahed"))//NaN
   ----------
    2. using by parseInt()=> ang data inside () convert to number if be number before text
    تقوم بفصل الرقم عن الكلام وتحويله إلى رقم بشرط أن  الرقم يكون قبل الكلام     
    المشكلة الثانية أنها دائما تعيد رقم صحيح بدون فاصلة عشرية 
    console.log(parseInt("4 mujahed"))//4(number)
     console.log(parseInt(" mujahed  5"))//Nan
     console.log(parseInt("5.5"))//5
     --------
     3. using by parseFloat()=> ang data inside ()   convert to number if be number before text
      نفس استخدام السابقة لمن تعيد الرقم مع فواصل عشرية 
     console.log(parseInt("5.5 mujahed"))//5.5(number)

   ````