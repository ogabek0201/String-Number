_<h1 align="center">JavaScript Lesson #2</h1>_

<p align="center">

<img src="https://img.shields.io/badge/Made%20by-Ogabek-yellow" >

<img src="https://img.shields.io/badge/Javascript-Method`s-white">

<img src="https://img.shields.io/badge/Method-String-brown">

<img src="https://img.shields.io/badge/Method-Number-brown">

<img src="https://img.shields.io/badge/Learn-Javascript-black">

</p>

---

__<center>A method is a block of code which only runs when it is called .</center>__

---
A method is a built–in command ("function", we'll talk about them later) that needs to be called to get a value. When using without parentheses, we get this function itself. As a rule, the browser will output it something like this: `"function methodName() { ... }"`.

```js

let txt="hello"
console.log(txt.methodName); //Function methodName(){ ... }
```

And to get the result, you need to call it by adding brackets:

```js
let txt="hello"
console.log(txt.methodName()); //Value
```

***

___<center> <h2>STRING METHODS</h2></center>___

*<center>when we use the string type with string methods, the string is converted to an array JavaScript supports various types of arrays, string array is one of them. A string array is nothing more than anything related to a string array.</center>*

* _There are 3 types of string creation:_
  * __double quotes__

    ```js
    ("hello")
    ```

  * __single quotes__

    ```js
    ('hello')
    ```

  * __Backticks__

    ```js
    (`hello ${hi}`)
    ```

---

## charAt()

 `The charAt method returns the character at a specified index position ) in a string`

* _Features:_
  * __The index of the first character is 0, the second 1, ...__

  ```js
  let txt="Ogabek"
  let result=txt.charAt(0)
  console.log(result) //O
  ```

  * __The index of the last character is string length-1__

  ```js
  let txt="Ogabek"
  let result=txt.charAt(txt.lenght-1)
  console.log(result) //k
  ```

  * __charAt gets the parameters__, and takes 1 argument

## concat()

* _Features:_
  * __The concat method joins two or more strings.__

  ```js
  let name="Ogabek"
  let surname="barotov"
  let fullName=name.concat(" ",surname)
  console.log(fullName) //Ogabek Barotov
  ```

  * __The concat method does not change the existing strings__

  ```js
  let name="Ogabek"
  let surname="barotov"
  let fullName=name.concat(" ",surname)
  console.log(surname) //Barotov
  ```

  * __The concat method returns a new string__

## replace()

`The replace method searches a string for a value or a regular expression`

* _Features:_
  * __The replace() method returns a new string with the value(s) replaced__

  ```js
  let txt = "visit grandpa"
  let txt2 = txt.replace("grandpa","grandma")
  console.log(txt2)//visit grandma
  ```

  * __The replace() method does not change the original string__

  ```js
  let txt = "visit grandpa"
  let txt2 = txt.replace("grandpa","grandma")
  console.log(txt)//visit grandpa
  console.log(txt2)//visit grandma
  ```

## replaceAll()

`The replaceAll method returns a new string with all matches of a pattern replaced by a replacement`

```js
let visit="My grandfather lives in the village. I'm going to visit my grandfather."
console.log(visit.replaceAll("grandfather","grandmother"));
//My grandmother lives in the village. I'm going to visit my grandmother.
```

## split()

```The split() method splits a string into an array of substrings```

* _Features:_
  * __The split() method returns the new array__

  ```js
  let txt="salom"
  let result=txt.split()
  console.log(result) //["salom"]
  ```

  * __The split() method does not change the original string__

  ```js
  let txt="My name is Ogabek"
  let result=txt.split(" ")
  console.log(txt) //My name is Ogabek
  ```

  * __If is used as separator, the string is split between words__

  ```js
  let txt="My name is Ogabek"
  let result=txt.split(" ")
  console.log(result) //["My", "name", "is", "Ogabek"]
  ```

## substr(start, length)

```The substr method extracts a part of a string```

* _Features:_
  * __The substr method begins at a specified position , and returns a specified number of characters__

  ```js
  let txt="salom people"
  let result=txt.substr(1,6)//start:1; lenght:6
  console.log(result) //alom p
  ```

  * __To extract characters from the end of the string , use a negative start position__

  ```js
  let txt="My name is Ogabek"
  let result=txt.substr(-6,6)
  console.log(result) //Ogabek
  ```

  * __The substr method does not change the original string__

## substring(start,end)

```go
The substring method extracts characters , between two indices (positions ), from a string , and returns the substring
```

* _Features:_
  * __The substring method extracts characters from start to end exclusive__

  ```js
  let txt="salom people"
  let result=txt.substring(1,6)//start:1; lenght:6
  console.log(result) //alom 
  ```

  * __Start or end values less than 0, are treated as 0.__

  ```js
  let txt="My name is Ogabek"
  let result=txt.substring(-6,6)
  console.log(result) //My nam
  ```

  * __If start is greater than end , arguments are swapped : (4, 1) = (1,4)__

  ```js
  let txt="minencraft"
  let result=txt.substring(4,1)
  console.log(result) //ine
  ```

  * __The substring method does not change the original string__

## slice(start,end)

```go
The slice() method allows you to return a new string that contains copies of characters cut from the original string.
```

* _Features:_
  
  * __the slice() method does not change the value of the string on which it was called.__

## toLowerCase()

```go
The toLowerCase method converts a string to lowercase letters
```

* _Features:_
  
  * __The toLowerCase method does not change the original string__

  ```js
  let txt='hello PEOPLE'
  let low=txt.toLowerCase()
  console.log(low);//hello people
  ```

## toUpperCase()

```go
The toUpperCase method converts a string to uppercase letters , using current locale
```

* _Features:_
  
  * __The toLowerCase method does not change the original string__

  ```js
  let txt='hello PEOPLE'
  let low=txt.toLowerCase()
  console.log(low);//hello people
  ```

## toLowerCase()

```go
The toLowerCase method converts a string to lowercase letters
```

* _Features:_
  
  * __The toUpperCase method does not change the original string__

  ```js
  let txt='hello PEOPLE'
  let upper=txt.toUpperCase()
  console.log(upper);//HELLO PEOPLE
  ```

## trim()

```go
The trim() method removes whitespace from both ends of a string.
```

* _Features:_
  
  * __The trim() method does not take in any parameters.__

  * __Returns a new string representing the str stripped of whitespace from both ends.__

  ```js
  let txt='         hello PEOPLE    '
  let tr=txt.trim()
  console.log(tr);//hello PEOPLE
  ```

  * __The trim() method does not change the original string.__

## includes()

```go
The includes() method checks if an array contains a specified element or not.
```

* _Features:_
  * The includes() method can take two parameters:
    * __searchValue__- The value to search for.
    * __fromIndex (optional)__ - The position in the array at which to begin the search. By default, it is 0.
  * The includes() method returns:
    * __true__ if searchValue is found anywhere within the array
    * __false__ if searchValue is not found anywhere within the array

```js
let txt='The position in the array at which to begin the search'
let search=txt.includes("array")
console.log(search);//true
```

## search()

```go
The search() method searches for a match between a given string and a regular expression.
```

* _Features:_
  * __The search() method takes a single parameter__
  * __Returns the index of the first match between the regular expression and the given string__

  ```js
  let txt='the position in the array at which to begin the search.'
  let search=txt.search("the")
  console.log(search);//0
  ```

  * __Returns -1 if no match was found.__

  ```js
  let txt='the position in the array at which to begin the search.'
  let search=txt.search("from")
  console.log(search);//-1
  ```

## toString()

```go
The toString() method returns the source code of the function as a string.
```

* _Features:_
  * __The toString() method does not take any parameters.__
  * __Returns a string representing the source code of the function.__

  ```js
  let num=99
  console.log(typeOf(num));//number
  let string=num.toString()
  console.log(typeof(string));//string
  ```

## repeat()

```go
The repeat() method creates a new string by repeating the given string a specified number of times and returns it.
```

* _The repeat() method takes in :_
  * ___count_ - An integer between 0 and +Infinity, indicating the number of times to repeat the string.__
  * __Returns a new string containing the specified number of copies of the given string.__

```js
let happy="happy holiday!"
let res=happy.repeat(2)
console.log(res);//happy holiday!happy holiday!
```

---
