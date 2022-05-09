## Add and Remove elements from array.

---

### Methods to add elements in an array.

1. ### push(valueOfAdd)

- appends values to an array. push is intentionally generic

- **Add element to last index in array.**

  إضافة عنصر في أخر مكان في المصفوفة

```

let array=['Mujahed','Mohammed','sam']

array.push('khaled')

array // ['Mujahed','Mohammed','sam','khaled']

array.push('khaled','Obad')//array=['Mujahed','Mohammed','sam','khaled','khaled','Obad']

أولا ننادي المصفوفة ثم نستخدم هذه method
```

2. ### unshift(valueOfAdd)

- appends values to an array. push is intentionally generic.

- **Add element to first index in array.**
  إضافة العنصر إلى أول مكان في المصفوفة

```

let array=['Mujahed','Mohammed','sam']

array.unshift('khaled')

array // ['khaled','Mujahed','Mohammed','sam']

array.unshift('khaled','Obad')//array=['khaled','Obad','Mujahed','Mohammed','sam','khaled']

أولا ننادي المصفوفة ثم نستخدم هذه method

```

---
### Methods to remove elements in an array.

1. ### pop()

* **removes the last element from an array and returns that value to the caller.**
تقوم بحذف أخر عنصر في المصفوفة 
وتحتفظ بقيمته بداخلها 

```
let array=['Mujahed','Mohammed','sam']

let elementRemove=array.pop() 
console.log(elementRemove)//'sam'

array // ['Mujahed','Mohammed']

كل مرة يعيد مناداتها تحذف اخر عنصر من جديد
```

2. ### shift()

*  **removes the first element from an array and returns that value to the caller.**

تقوم بحذف أول عنصر في المصفوفة وتحتفظ بقيمته بداخلها 

```
let array=['Mujahed','Mohammed','sam']

let elementRemove=array.shift() 
console.log(elementRemove)//'Mujahed'

array // ['Mohammed','sam']

كل مرة يعيد مناداتها تحذف أول عنصر من جديد
```