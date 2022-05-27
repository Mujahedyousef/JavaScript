## concat( )
>  method is used to merge two or more arrays. This method does not change the existing arrays, but instead returns a new array.

هذه ال method تقوم بعمل دمج بين ال Arrays
وتعيد مصفوفو جديدة ويممكن إضافة عدد كبير من المصفوفات 
ويمكن اضافية كلام وعناصر الى المصفوفة 

```
const array1 = ['Mujahed', 'fayeq', 'hitham'];
const array2 = ['yahea', 'mousa', 'abdallah'];

1. array1.concat(array2)
 ['Mujahed', 'fayeq', 'hitham','yahea', 'mousa', 'abdallah']

//يمكن الحفظ بمتغير جديد 
2. const array3 = array1.concat(array2);
console.log(array3);
['Mujahed', 'fayeq', 'hitham','yahea', 'mousa', 'abdallah']

3.يمكن اضافة اي شئ الى المصفوفة 

const array3 = array1.concat(array2,"kkkkk");
console.log(array3);
['Mujahed', 'fayeq', 'hitham','yahea', 'mousa', 'abdallah',"kkkkk"]

4.يمكن اضافة اكثر من مصفوفة

const array3 = array1.concat(array2,array4,array5,array6);

```

-------------

## join( )

> the method creates and returns a new string by concatenating all of the elements in an array (or an array-like object), separated by commas or a specified separator string. If the array has only one item, then that item will be returned without using the separator.

تقوم بعرض محتويات المصفوفة وتحويلها إلى نص string

يمكن تحويل الفواصل بين العناصر الى اي رمز 

```
const array1 = ['Mujahed', 'fayeq', 'hitham'];

1 - console.log(array1.join())
//Mujahed,fayeq,hitham سيتم الغرض  نص 

2. console.log(array1.join(''))//Mujahedfayeqhitham
تعني انه قم بحذف مكان كل فاصلة تفصل بين العناصر  

3. console.log(array1.join('#'))//Mujahed#fayeq#hitham
يقوم باستبدال الفاصلة بين العناصر الى اي رمز وضع هنا 




```
