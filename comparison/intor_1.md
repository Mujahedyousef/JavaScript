
هنا أريد المقارنة بين قيم المتغيرات
دائما تعيد لنا المقارنة قيمة boolean

true || false

```
let x="mujahed"
let y="ahmad"
let z="mujahed"
console.log(x===y)// false
console.log(x===z)// true
```

في أغلب الاحيان نطلب من المستخدم إدخال قيمة
فنتحقق من هذه القيمة من خلال المقارنة مع البيانات المخزنة مسبقاً

هنا نستخدم بعض الأساليب لحصر واخذ القيمة الصحيحة من المستخدم

* .toUpperCase( )

هنا تقوم بتغير جميع الحروف المدخلة الى حجم كبير

* .toLowerCase( )

 هنا تقوم بتعديل جميع الحروف المدخلة الى حجم صغير

* .trim( )

 هنا تقوم بحذف الفراغات قبل او في نهاية الكلام  

* prompt(`enter your email`) 

تستخدم من جانب الwindow
ليقوم المستخدم بإدخال قيمة معينة 

```
let email="mujahedyousef97@yahoo.com"
لنفرض أن هذه القيمة محفوظة لدي في 
Database


let askUser=prompt(`please, Enter your email`)
askUser=" MujahedYousef97@yahoo.com"
هنا اطلب من المستخدم أن يقوم بإدخال الايميل 
الخاص به لاسمح له بالدخول 

من بعد المقارنة والتأكد انه مخزن لدي ولديه حساب 

يمكن ان يقوم المستخدم بإدخال حروف كبيرة 
او فراغات بداية الكلام او في نهايته 

ولكي أقوم بأخد القيمة المدخلة بالشكل الذي اريده استخدم بعض 
methods

console.log(email===askUser)//false

console.log(email===askUser.toLowerCase().trim())//true

قمت بحذف مسافة البداية لان الفراغ يعتبر حرف وقمت بتصغير جميع الحروف 
فأصبحت القيم متساوية 
```
----

[javascript-operators](https://www.tutorialsteacher.com/javascript/javascript-operators)

(==)تقارن الvalue فقط 
(===)تقارن الvalue , data type 