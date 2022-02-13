In this post , we will discuss about the DOM and its properties . We will also see the some properties
 to manipulate the DOM ( Document Object Model  ) .

## What is DOM ( Document Object Model ) ?

HTML is used to structure the page and JavaScript is used to add behaviour to our web page but 
when an HTML file is loaded in browser , JavaScript can not understand the HTML tags like 
```<a> <h1> 
```  directly and can not perfom the task . So , A HTML node is created . As a name suggest 
Document Object Model ( DOM ) is just the same document but with object (node). Now Javascript 
can understand the ```h1  a```  and we can perform the task like  ```document.body ```.

Basic Structure of Html as following 



```
<!DOCTYPE HTML>
<html>
<head>
  <title> 
Hello  //text node
</title>
</head>
<body>
  World   //text node
</body>
</html>


```
 > Every HTML tag is an object and nested tags are its children. When we write some text inside
it is a text node.


![dom.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1644763578563/OwJkIH_Lg.gif)

above is an example of DOM Tree. In above when we write the class of an element it also comes as 
children . Now we will see how to manipulate the DOM? Generally, we do two things with the Dom 
we get the element and its properties or we set the element .


```
<!DOCTYPE HTML>
<html>
<head>
  <title> 
Hello  //text node
</title>
</head>
<body>
<div>
<div>
<span>  
 </span>
<script src="src/index.js">
</body>
</html>

```

- Add  a ```<script></script>``` element just above the closing ```</body>``` tag and write 
the code .
- We get the reference of a span and store it in a variable .
-   Add the text inside the span 

```
const divRef = document.querySelector('div');
divRef.innerText = " hello  "  //add text inside the span

```
Creating And Removing 

- we get the reference of span .

```
const span = document.querySelector('span'); 


```


- we create the ```<p>``` tag and add text 


```

const para = document.createElement('p') ;

para.innerText = " Hello World   " ;

```

- Now we add ```<p>``` inside the ```<span>``` tag by  ```.appendChild``` 

```
span.appendChild(para) ;

```
 - Remove the ```<p>``` tag we create above 

```
span.removeChild(para) ;

```

Now that's all for this post there a lot more .
