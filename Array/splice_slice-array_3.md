# splice and slice array
-----
## splice(start, remove count,add,add,....)

تؤثر على المصفوفة الاصلية 

- Is a built-in method for JavaScript Array objects.

  - It lets you change the content of your array by removing or replacing existing elements with new ones.

 تمكننا من حذف عناصر أول إضافة عناصر جديدة من خلال تحديد المكان من خلال start
 وتحديد عدد العناصر المراد حذفها اعتماداَ على start
 وparameter الثالث يساوي القيم المراد إضافتها إعتمادا على الموقع المحدد 

  - This method modifies the original array and returns the removed elements as a new array

   تغيير على ال array نفسها 
  بحيث يمكن الإستفادة من القيم المحذوفة 


```
let array=['Mujahed','Mohammed','sam']

array.splice(start location (index), number element i want remove , value to adding , add , add as i want)

حذف فقط 

array.splice(1,1)سيذهب الى موقع البداية ثم يرى كم عنصر اريد ان احذف وينفذ
ثم يحذث التغيير على المصفوفة نفسها 
['Mujahed','sam']
-------
حذف وتبديل 
array.splice(0,1,"hello")//تعني إذهب على العنصر الاول ثم إحذف قيمة واحد ومن ثم قم بإضافة العنصر الجديد مكان البداية المحددة 

['hello','Mohammed','sam']
----
إضافة بدون حذف 


array.splice(1,0,"my","name")
سيذهب الى نقطة البداية المحددة ولم يحدد عناصر للحذف ثم يقوم بإضافة العناصر الجديدة موقع العنصر المحدد

['Mujahed',"my","name",'Mohammed','sam']
------

يمكن حفظ القيمة المحذوفة أو القيم المحذوفة 
داخل متغير واستخذامها

let element=array.splice(1,2) //["my","name"]

```

-----

## slice(start, end not include )

* Returns a shallow copy of a portion of an array into a new array object selected from start to end ( end not included) where start and end represent the index of items in that array.

لا تحدث إي تغيير مباشر على ال array 
لكن تقوم بعمل نسخة منها من العناصر المراد تطبيقها عليهم يعني ترجع array جديدة 

```
let array=['Mujahed','Mohammed','sam',"mazen"]

array.slice(start location, end not include)البداية عداد index

let new=array.slice(0,2) //['Mujahed','Mohammed']

لو حاول طباعة array  ستكون كما هي بدون أي تغيير 

-----------
يمكن نسخ المصفوفة بالكامل أو بتحديد البداية فقط وهو يمكل الى النهاية 



let new=array.slice(1)
['Mohammed','sam',"mazen"]
-----------
يمكن أن تأخذ قيم سالبة بحيث يبدأ القطع من اليمين إلى اليسار 
مع العلم دائماَ أخر قيمة في المصفوفة -1 

let new=array.slice(-3,-1)//['sam',"mazen"]
  0           1          2     3       يسار الى يمين 
    -4        -3         -2      -1   يمين إلى يسار
['Mujahed','Mohammed','sam',"mazen"]
```