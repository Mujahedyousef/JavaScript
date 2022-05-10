#  sort and reverse array.
-----
## reverse()

* The reverse() method reverses the order of the elements in an array.

* The reverse() method overwrites the original array.

يقوم بعكس ترتيب المصفوفة الرئيسية 

```
let array=[1,5,8,9]
array.reverse()//[9,8,5,1]

```
-----
## sort()

* sorts the elements of an array.

* overwrites the original array.

* sorts the elements as strings in alphabetical and ascending order.

يقوم بترتيب عناصر المصفوفة تصاعداَ والكلام أبجديا
ويعدل على نفس المصفوفة 

```
let array=[1,10,16,5,8,9]
let array_2=['Muj','Amj','za','ya']
array.sort()//[1,5,8,9,10,16]
array_2.sort()//['Amj','Muj','ya','za']
```