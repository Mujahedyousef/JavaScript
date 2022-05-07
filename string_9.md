## String control in javascript

> the string is a sequence value that means each element is stored in a specific place for him, and the space has a value

هي قيمة تسلسلية تعني تخزين العناصر بشكب متتابع في أماكن محدده لها ، الفراغ له قيمة

1.  repeat( )

    > can repeat the text sentence as many times as you pass it to her.

             "Mujahed".repeat(2)//"MujahedMujahed"

2.  length

    > You can find the number of a text string and return the number of characters.

         "Mujahed".length//7
         "Mujahed ".length//8 space
        يمكنك من  معرفة عدد السلسلة النصية و ارجاع عدد الاحرف

3.  Getting to the character

    1. To access a specific index in any text string, write the variable name and then the desired character number in square brackets.
       ```
       "Mujahed"[2]//"j"
       let name="hello"
       name[1]// "e"
       للوصول الى index معين في اي سلسلة نصية تكتب اسم المتغير ثم رقم الحرف المراد في الاقواس المربعة
       ```
    1. charAt( index)

       Using charAt to get to the desired character and to get to it we pass the desired index

       ```
       let name="mujahed";
       name.chartAt(2)//"j"

       للوصول الى الحرف المراد و للوصول له نمرر ال index
       ```

       الفرق بين الطريقتين
       عند كتابة index
       غير موجود في الطريقة الاولى ترجع undefind

       أما الطريقة الثانية لا ترجع شيئاً

---

## Find character in text strings

> indexOf( )

1. indexOf("character")

   > Through this method, you can search for any character or text in any text string from the beginning of the text string, by passing the character you want to search for, and then return to you the index number if it exists.

   من خلال هذا ال method يمكنك البحث عن اي حرف او نص في اي سلسلة نصية من باداية السلسلة النصية و ذلك من خلال تمرير الحرف المراد البحث عنه و من ثم يرجع لك رقم ال index اذا كان موجود

   ```
   let name="hello world";
   name.indexOf("l")//2
   name.indexOf("world")//6
   في الكلمة عند أول حرف
   سيقوم بإعادة مكان
   ( index)
   أول حرف تم البحث عنه من اليسار اليمين مع تضمين الفراغات في العد
   ```

2. indexOf("character",index)

   > Search from the desired place in the text string by passing the start point of the search.

   البحث من المكان المراد في السلسلة النصية و ذلك من خلال تمرير نقطة بداية البحث

   ```
   let name="hello world";
   name.indexOf("l",4)//9
   هنا حددت نقطة وموقع بداية البحث
   سيبدأ البحث من المكان رقم 4
   وأول مكان يجد فيه الحرف يعيد فيه موقعه مع تضمين الفراغات في العد
   ```

   ***

> lastIndexOf( )

1. lastIndexOf("character")

   > You can search from the end of the text string through lastIndexOf()

   البحث من نهاية السلسلة النصية

   ```
     let name="hello world";
    name.lastIndexOf("l")//9
    بدء البحث من اليمين إلى اليسار
    وأول ما وجد أول حرف مشابه له أرجع موقعه
   ```

1. lastIndexOf("character",index)
   > You can search from the desired place in the text string by passing the start point of the search.
   ```
   let name="hello world";
   name.lastIndexOf("l",7)//3
   راح يمشي بشكل تنازلي من اليمين لليسار
   يعني لو كان بداية البحث من 3
   بس راح يشيك على 2و1و0
   ```

---

> slice( )

- During this method, you can chop the text string and return what you want from it by passing the index number at the beginning of the slicing and the index number at the end of the slicing, and so it returns the cut part of the text, and if you do not pass any numbers, the index will return the whole text.

  ```
  let name="hello world";
  بدون وضع بداية التقطيع سيعيد النص كامل
   1. name.slice()//"hello world"

   عند وضع مكان بداية التقطيع
   يكون موقع البدية متضمن الاعادة
   2. name.slice(2)//"llo world"

   عند وضع بداية ونهاية التقطيع
   سيتضمن البداية ولن يتضمن النهاية
   2. name.slice(2,5)//"llo" (سيبدأ من 2 ويأخذها وينتهي عن 4 ويأخذها ولن يأخذ 5)
   وهي عبارة عن عدد الأحرف بين البداية والنهاية 
   slice(1,10)==10-1=9
    سيظهر 9 أحرف 
  ```
----
> split( )
 * Returns a copy of the String in the form of an array.

  ترجع نسخة من الـ String على شكل مصفوفة و اذا تم مرير لها حرف تقوم باقتطاع هذه السلسلة النصية من مكان هذا الحرف في النص

  ````
  let name="hello world in javaScript";
  1. name.split(' ')//["hello", "world" ,"in" ,"javaScript"]// راح يعمل قطع عند كل فراغ ويحفظهم داخل مصفوفة كعناصر 
  ------
  2. name.split('')// ['h','e','l','l','o'......]
  هنا سيعتبرها حرف ويثطع عند كل حرف
  -------
  3.  name.split('l')// ['he', '', 'o wor', 'd in javaScript']
  راح يقطع من عند هذا الحرف 
  -----
  4. name.split('',3)//['h','e','l']
  هنا استطيع تحديد عدد المرات التي اريد ان يقوم بالقطع فيها يطبقها ولا يعيد الباقي

  ````
  ----------
  