## Concatenation
* Three ways to do that.

    1. The + Operator
    > The same + operator you use for adding two numbers can be used to concatenate two strings.
     ````
     const str = 'Hello' + ' ' + 'World';
     str; // 'Hello World'
     بنعمل دمج من خلال علامة (+) للمتغيرات 
    ------------
    another way

    et str = 'Hello';
    str += ' ';
    str += 'World';
    str; // 'Hello World'
     ````
    -----
     2. Array # join( )==>method for arrays

    نستخدم method خاصة ب ال arrays
    * The Array#join() function creates a new string from concatenating all elements in an array. For example:
    ````
    ['Hello', ' ', 'World'].join(''); // 'Hello World'

     ما يوضع داخل ال 
     join()
     هو ما يحدد شكل الدمج 
     هنا ادمج كل العناصر معا 
    ````
    * The first parameter to join() is called the separator. By default, the separator is a single comma ','.
    ````
    ['a', 'b', 'c'].join(); // 'a,b,c' 
    هنا ادمج جميع عناصر المصفوفة بدون تقسيمات 
    ````
    * You can pass in any separator you want. Separators make Array#join() the preferred choice for concatenating strings if you find yourself repeating the same character over and over again. For example, you can use ' ' as the separator to join an array of words:
    ````
    // 'Twas the night before Christmas'
    ['Twas', 'the', 'night', 'before', 'Christmas'].join(' ');
   هنا الدمج عند كل فراغ 
    ````
   * you can use '/' to join together URL fragments:
   ````
   // 'masteringjs.io/tutorials/fundamentals/string-concat'
   ['masteringjs.io', 'tutorials', 'fundamentals', 
    'string-concat'].join('/');
    هنا أريد أن اضع بعد كل عنصر 
    /
    ويعيدها ك 
    string
     كاملة 
   ````
   -----
   3. String#concat() ==> Using for string 
    
    الطريقة الثالثة باستخدام 
    method مختلفة 
    يمكن استخدامها مع النصوص 
    والمتغيرات 
   > The concat() function takes one or more parameters, and returns the modified string. Strings in JavaScript are immutable, so concat() doesn't modify the string in place.
   ````
   const str1 = 'Hello';
   const str2 = str1.concat(' ', 'World');
   
   // 'Hello'. Strings are immutable, so `concat()` does not modify `str1`
   str1;
   // 'Hello World'
   str2;
   للعلم تعيد مصفوفة جديدة بعد الدمج 
   
   ````
   * Backticks are an ES6 feature that allows you to create strings in JavaScript.
   من خلال
   
    ` ${متغيرات بحيث ستأخذ القيمة وتعوضها  }`
   ````
   let name="mujahed"
   let age=25
   console.log (`My name is ${name} and my age is : ${age} `) //My name is mujahed and my age is : 25
   ````
   ------
   