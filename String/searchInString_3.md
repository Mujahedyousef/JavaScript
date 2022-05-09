# Searching texts in javascript.

## We have many ways to search texts in javascript

- They are all searching in texts but they are different from each other

1. indexOf( )
1. lastIndexOf( )
1. includes( )
1. startsWith( )
1. endsWith( )

جميعهم يقومون بالبحث لكن هناك إختلافات

---

## indexOf( )

- During this method, you can search in texts from the beginning of the text by passing the letter or text to be searched for, and it returns the index value of the letter or text if it is found, and if the letter does not exist, it returns -1.

إذا لم تجد العنصر ترجع -1
```
indexOf("character")// إبدأ البحث من البداية

indexOf("character", starter search location)(اختياريه)
indexOf("m" , 5)=> معناها إبدأ البحث عن موقع أول
  a حرف
  تجده وبداية البحث من المكان المذكور
  وعند إيجاده أرجع مكانه
  
let name="hello everyone"
name.indexOf("l")//2
name.indexOf("o",5)//11 //سيبدأ البحث من 5 إلى الاخير 
```
----

## lastIndexOf( )

- Through this method, you can search the texts from the end of the text by passing the letter or text to be searched for, and it returns the index value of the letter or text if it is found, and if the letter does not exist, it returns -1.

تبدأ البحث من النهاية من( من  اليسار إلى اليمين )
وأول حرف مشابة تعيد موقعه 

إذا لم تجد العنصر ترجع -1
`````
 lastIndexOf("character")// إبدأ البحث من البداية

 lastIndexOf("character", starter search location)(اختياريه)
 lastIndexOf("m" , 5)=> معناها إبدأ البحث عن موقع أول
  a حرف
  تجده وبداية البحث من المكان المذكور
  وعند إيجاده أرجع مكانه

let name="hello everyone"
name.lastIndexOf("l")//3 راح يبدأ البحث بالعكس من اليمين الى اليسار

name.lastIndexOf("o",6)//4
يبدأ البحث من 6 ويكمل البحث بإتجاه اليمين 


`````

----

 ## includes( ) 


* Through this method, you can search in texts by passing the character or text to be searched, and it returns true if it is found and false if the character does not exist.

هنا تقوم بالبحث على العنصر وتكون القيمة الراجعة إما true ||flase

```
includes("character")//يبدأ البحث  من البداية 
includes("character", starter search location)//راح يبدأ البحث من المكان المحدد باتجاه اليمين متجاوز السابق  

let name="hello everyone"
name.includes("l")//true
name.includes("l",5)//false 

```
---

## startsWith( )
Through this method, you can find out the letter that any text begins with, by passing a letter to it. It can return true if the text begins with this letter or return false in case the letter is wrong, and you can start the search from the desired place in any text.

   تقوم بالتأكد من أن بداية الكلمة تبدأ بحرف معين 
وتعيد true || false

````
startsWith(character)//  راح يشوف أول حرف بأول كلمة فقط ويمكن البحث عن كلمة كاملة وسيتأكد من أول حرف لها فقط 

startsWith(character,starter search location) //سيتأكد من أول حرف من من بداية البحث 

let name="hello everyone"
name.startsWith("h")//true
name.startsWith("l")//false
name.startsWith("l",3)//true 
name.startsWith("everyone",6)//true 


````





---

## endsWith( ) 

* During this method, you can find out which character any text ends with, by passing the number of characters to be searched, and it can return true if the text ends with this character or return false in case the character is wrong.

هنا راح يشوف أخر حرف بالجملة كلها ويتأكد منه true || false
 وفيها ميزة إضافية أنها تأخذ رقم وهو رقم العناصر المراد معرفة أخر حرف بها 

````
endsWith(character)// راح يروح لاخر حرف أخر عنصر بكل الجملة 

endsWith(character,length) هون راح يبدأ العد من البداية حتى يصل الى length ويتأكد منه
والعد يبدأ من 1 لاني أقوم بحساب طول أعد العناصر 
let name="hello everyone"
name.endsWith("e")//true
name.endsWith("o")//false
name.endsWith("l",3)//true 
name.endsWith("v",8)//true يقوم بعد 8 عناصر ويتأكد من الحرف 

````