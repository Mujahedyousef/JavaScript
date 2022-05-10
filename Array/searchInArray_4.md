# Search in array
----
## indexOf("value",start)

* returns the position of the first occurrence of a value in a string. The indexOf() method returns -1 if the value is not found.

يرجع موقع التكرار الأول وإن لم يجد يرجع -1 
يمكن أن يأخذ parameter إضافي يحدد مكان البدأ 

```

let array=['Mujahed','Mohammed','sam','Mujahed']

array.indexOf('sam')//2

array.indexOf('mo')//-1

array.indexOf('Mujahed',1)//3  

لأن مكان البحث يبدأ من 1


```

-----

## lastIndexOf("value",start)

* the method returns the last index at which a given element can be found in the array, or -1 if it is not present.

تبدأ البحث من نهاية المصفوفة 
من اليمين إلى اليسار 
يمكن أن تأخذ موقع باية البحث أيضا

```

let array=['Mujahed','Mohammed','sam','Mujahed',"Mohammed"]

array.lastIndexOf()//4

array.lastIndexOf('mo')//-1

array.indexOf('Mujahed',2)//0 
  هنا لأن بداية البحث محدد وهذه الطريقة تكمل من اليمين إلى اليسار تكل طريقها حتى تجد أول  عنصر مشابة وترجع موقعه

array.indexOf('Mujahed')//3 

array.indexOf('Mujahed',-2 )//0 

```

-----
## includes("value",start)

* the method determines whether an array includes a certain and return true or false.

تبحث في المصفوفة عن العنصر وتعيد صح أو خطأ 
ويمكن أن نحدد قيمة وموقع بداية البحث

```

let array=['Mujahed','Mohammed','sam','Mujahed']



array.includes('mo')//false

array.includes('Mujahed',2)//true 
 
array.includes('Mohammed',2)//false 



```