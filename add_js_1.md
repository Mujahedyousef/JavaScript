# How to add javascript codes?

> First of all, the tag responsible for adding JavaScript codes to a web page is the
> `<script>` tag.

> First method

- You can write javascript directly in the html file
  This is done by writing between the beginning and the end of the `'<script></script>` tag.

```
<script>
document.write(“hello world”);
</script>
```

> Second method

- You can link an external javascript file to the html file
  This is also done through the `<script>` tag and using the src property to link files together.

```
<script src=“main.js”></script>
```

- You can write javascript code anywhere in your file
  You can write it in the head and you can write it in the body
  But you should know that order is important
  So if you are going to write something in javascript that affects an element in the body
  You must write this command after the desired element, not before it, so that no errors occur
  But you can solve this problem through the

```
onload event
```
