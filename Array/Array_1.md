# Array

> Storing a collection of multiple items under a single variable name, and has members for performing common array operations.

. مجموعة من العناصر مخزنة في مواقع متجاورة لها نفس اسم المتغير

- The idea is to store multiple items of the same type together. This makes it easier to calculate the position of each element by simply adding an offset to a base value, i.e., the memory location of the first element of the array (generally denoted by the name of the array). The base value is index 0 and the difference between the two indexes is the offset.

الهدف منها هو تخزين مجموعة من العناصر المتشابهة في النوع نفسه
.والقدرة على معرفة مكان كل واحدة وتحديد موقعها من خلال العداد index

## Types of indexing in an array:
````
let array =[1,5,6,8,7,"m",true,NaN,null,undefined]
````
1. 0 (zero-based indexing): The first element of the array is indexed by a subscript of 0.

أول عنصر في المصفوفة

````
console.log(array[0])//1 
````
2. (n -1): last index in the array equal length the array -1 

````
console.log(array[10-1])//undefined 
````
----

## Advantages of using arrays: 

1. Arrays allow random access to elements. This makes accessing elements by position faster.

تسمح بالوصول العشوائي إلى العناصر وهذا يعطيها سرعة بالحصول على الموقع للعنصر

2. Arrays have better cache locality which makes a pretty big difference in performance.

لها منطقة تخزين مؤقت مما يجعلها مما يجعل أدائها أفضل 

3. Arrays represent multiple data items of the same type using a single name.

تمثل عناصر بيانات متعددة من نفس النوع باستخدام اسم واحد.

-----
## Disadvantages

1. You can’t change the size i.e. once you have declared the array you can’t change its size because of static memory allocation.

لا يمكن تغيير حجمها بعد إعلانها لأنه يتم تخصيص لها ذاكرة ثابتة 

2. Insertion(s) and deletion(s) are difficult as the elements are stored in consecutive memory locations and the shifting operation is costly too.

تكون عملية الإدراج والحذف صعبةلأنه  يتم تخزين العناصر في مواقع ذاكرة متتالية وعملية النقل مكلفة أيضًا.

3. 

----

## Applications on Array

1. Array stores data elements of the same data type.

لتخزين عناصر من نفس النوع 

2. Used in solving matrices problem

لحل مشكلة المصفوفات

3. Applied as a lookup table in computer.

كجدول بحث في الكمبيوتر

4. Databases records are also implemented by the array.

تنفيذ سجلات قواعد البيانات بواسطة المصفوفة

5. Helps in implementing sorting algorithm.

يساعد في تنفيذ خوارزمية الفرز.

6. Different variables of the same type can be saved under one name.

حفظ المتغيرات المختلفة من نفس النوع تحت اسم واحد.

7. Arrays can be used for CPU scheduling.

استخدام المصفوفات لجدولة وحدة المعالجة المركزية.

8. Used to Implement other data structures like Stacks, Queues, Heaps, and Hash tables.

يُستخدم لتنفيذ هياكل البيانات الأخرى مثل جداول المكدس وقوائم الانتظار والأكوام والتجزئة.

----

## Nested Array 

> In JavaScript is defined as an Array (Outer array) within another array (inner array).

هو وجود مصفوفة بداخل مصفوفة 

````
let array =[1,5,6,8,7,5,[10,[12,null]],undefined]

when I want to get element 12 

array[6][1][0] now i get it 

scop inside scop inside scop .
````
----

## Assigning Values to Array Elements
* We can assign a new value in an array or re-assign or change the value already found.

يمكننا إعطاء قسمة لعنصر أو إعادة وتغير القيمة لعنصر موجود 


````
1. when we want to invoke to an array

nameOfArray // 
----------------
2. when we want to invoked to array and get specific element

nameOfArray[index of element]
-----------
let array =[1,5,6,8,7,5,undefined]
 
array[7]="why"//[1,5,6,8,7,5,undefined,"why" ]
هنا قمت بإدخال قيمة جديدة من خلال تحديد موقع  المراد إضافته فيه وهو بعد أخر عنصر موجود بالفعل

array[5]="mujahed"//[1,5,6,8,7,"mujahed",undefined,"why" ] 

هنا قمت بالتعديل على قيمة موجودة فعليا


````
----