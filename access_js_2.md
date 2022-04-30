## JavaScript can access three places to edit.

1.  HTML page.

- Through the document command, this command allows you to access the html page to modify it and add what you want

```
document.write("hello ")
```

2. The console

- Accessing the console part through the console command in JavaScript

```
console.log("hello")
```

3. The Browser

- Modify the browser through the window command in javascript.

```
window.alert("hello" )
```

---

## The difference between the document - console - window

### Document

1. The document is the programmatic command responsible for accessing the html page

1. When you create an html page, the browser sees it as follows

1. At first it creates a document and from it makes the html tag

1. And then it does the head and body and what's inside them

عند عمل صفحة html المتصفح يقوم بعمل document ويضع بداخله صفحة html  
ثم يقرأ ما دلحل هذه الصفحة بالترتيب
فيمكن الوصول لأي شئ بداخل صفحة html عن طريق document

```
                    document(see first)
                         HTML(second)
                         head || body
                meta && title || tags

```

### Console

- You can write code commands in your code editor and also in the console part that is available in all browsers. You can also control the console part through JavaScript via the console command.

يمكن كتابة أي كود مباشرة ومشاهدة النتيجة فورا وهو بالأساس object
بداخله أوامر يمكن تنفيذها

---

### Window

- You can also modify the browser through the window command in JavaScript.

  يعني التحكم في المتصفح كامل وهو يشمل التحكم في ال 

  console و document

  جميع الأوامر الموجودة في
  js متوفرة في browser
  استطيع التحكم في ال window بدون كتابتها قبل الكلام لأن المتصفح لوحده يستطيع الفهم أنني الان في المتصفح

---

في النهاية جميعها
object ولديهم مجموعة أوامر يمكن تطبيقها
