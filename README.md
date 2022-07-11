# html-silicium

*By Default first render index.html then other files like index2.html and so on*

*Html files has .html extension like home.html and index.html*

__Every html file has a format like this :__
```
DOCTYPE -> represent a html file
html
    head -> an information that use by bots

    body -> an information that end user see
html
```

__Like this :__
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title></title>
</head>
<body>
    
</body>
</html>
```

*Some tags in html files have open and close tags like html(&lt;html&gt; to open and &lt;/html&gt to close it ) and some tags open and close tag in one tag like meta( &lt;meta&gt; )*

*In body tag we can show anything that user sees*

---

*&lt;meta charset="UTF-8"&gt; shows that we want use UTF-8 for encoding(without this , persian words dosent show carefully*

---

*&lt;title&gt;Anything you want&lt;/title&gt; shows tab name(Anything you want) in browser*

---

*Note: HTML is skelton our webpage but CSS can beautiful this skelton*

**In html files we have tags . Each tag represent a diffrent thing:**

*Heading tags are h1,h2,h3,h4,h5,h6(h1 have biggest text and h6 have smallest text) like &lt;h1&gt;Anything you want&lt;/h1&gt;*

*To use pragraph tag we can use p tag like &lt;p&gt;Anything you want&lt;/p&gt;*

*Some tags line p , h1 to h6 , div , article , header goes our content to newline but some other tags like a , img , span , b , i , strong modify our content in that like* 


*To Bold our content we can use b tag like &lt;b&gt;Anything you want&lt;/b&gt;*

*To italic our content we can use i tag like &lt;i&gt;Anything you want&lt;/i&gt;*

*Link tag shows with a tag and used for linking . In href attribute we can set after click goes where. like &lt;a href="https://google.com"&gt;Google&lt;/a&gt;*
+ You can use target attribute in link tag to open in tab with set &lt;a href="https://google.com" target="_blank"&gt;Google&lt;/a&gt; 

*To use image in our page , we can use img tag like &lt;img src="Address image" &gt;*
+ Note: img tag dosen't have close tag .
+ Note: you can use relative address or internet address to link your image .

*With span tag , you can select part of our element . So in css we will teach how to change style of that part .* 

*With strong tag we can bold our text , but the diffrence to b tag is b is strong is emphizized to search engines .*

**With div tag , we can break our website into multiple section**

*With hr tag , we can create a line in our page*
*With br tag , send content to newline*
+ Note: hr & br tag dosen't have close tag .

---

*Every html files have many sections . like this :*
+ Header
+ Main
    + Main-section1
    + Main-section2
    + Main-section3
+ Aside
    + Asider-section1
    + Asider-section2
    + Asider-section3
+ Footer

> In directory 2 , we create this template

---

**We have several types of lists**
1. unordered list
    + Unorderd list shows with ul tag
    + Every elements of list shows with li
    + Example:
    ```
    <ul>
        <li>One</li>
        <li>Two</li>
        <li>Three</li>
    </ul>
    ``` 
2. ordered list 
    + Oorderd list shows with ol tag
    + Every elements of list shows with li
    + Example:
    ```
    <ol>
        <li>One</li>
        <li>Two</li>
        <li>Three</li>
    </ol>
    ``` 
> We can use ordered list and unordered list with together

> In directory 3 , we used these lists .

---

**To create a table , we can use table tag**
+ To create every row in table , we can use tr tag
+ To create an element in row , we can use td tag
    + But for header of table , better to use th tag instead of td tag

*Here an example of table :*
```
<table>
        <tr>
            <th>ID</th>
            <th>Name</th>
            <th>Price</th>
        </tr>
        <tr>
            <td>1</td>
            <td>Meat</td>
            <td>100000 T</td>
        </tr>
        <tr>
            <td>2</td>
            <td>Juice</td>
            <td>3000 T</td>
        </tr>
</table>
```

> In directory 4 , we used this table .

---

**With form tag we can get some information from user and process these data.**

*There are many types elements that we can use them in our pages:*
1. text input
    + placeholder shows a text in input when user dosen't fill the input
    + we can use label tag for every element of form
    + Example:
    ```
    <form>
        <label>Name :</label>
        <input type="text" name="Name" placeholder="Name">
    </form>
    ```
2. email input
    + Example:
    ```
    <form>
        <label>Email :</label>
        <input type="text" name="Email" placeholder="Email">
    </form>
    ```
3. texterea
    + We can set rows and cols of texterea
    + Example:
    ```
    <form>
        <label>Content :</label>
        <textarea name="Content" cols="30" rows="10" placeholder="put your content"></textarea>
    </form>
    ```
4. radio input
    + When we set the same name for our radio inputs , we can just select one of them
    + Example
    ```
    <form>
        <div>
            Enter your gender : 
            <label>Male</label>
            <input type="radio" value="male" name="gender">
            <label>Female</label>
            <input type="radio" value="female" name="gender">
            <label>None</label>
            <input type="radio" value="none" name="gender">
        </div>
    </form>
    ```
5. checkbox
    + Example:
    ```
    <form>
        <div>
            Enter your favaroites : 
            <label>Football</label>
            <input type="checkbox" name="Football">
            <label>Tenis</label>
            <input type="checkbox" name="Tenis">
            <label>Basketball</label>
            <input type="checkbox" name="Basketball">
        </div> 
    </form>
    ```
6. select
    + Example:
    ```
    <form>
        <div>
            Enter your city : 
            <select name="city">
                <option value="tehran">tehran</option>
                <option value="tabriz">tabriz</option>
                <option value="shiraz">shiraz</option>
            </select>
        </div>
    </form>
    ```
7. submit button
    + With submit button , we can send our form 
    + Example:
    ```
    <form>
        <label>Name :</label>
        <input type="text" name="Name" placeholder="Name">
        <br>
        <label>Email :</label>
        <input type="text" name="Email" placeholder="Email">
        <br>
        <label>Content :</label>
        <textarea name="Content" cols="30" rows="10" placeholder="put your content"></textarea>
        <br>
        <div>
            Enter your gender : 
            <label>Male</label>
            <input type="radio" value="male" name="gender">
            <label>Female</label>
            <input type="radio" value="female" name="gender">
            <label>None</label>
            <input type="radio" value="none" name="gender">
        </div>
        <br>
        <div>
            Enter your favaroites : 
            <label>Football</label>
            <input type="checkbox" name="Football">
            <label>Tenis</label>
            <input type="checkbox" name="Tenis">
            <label>Basketball</label>
            <input type="checkbox" name="Basketball">
        </div> 
        <div>
            Enter your city : 
            <select name="city">
                <option value="tehran">tehran</option>
                <option value="tabriz">tabriz</option>
                <option value="shiraz">shiraz</option>
            </select>
        </div>
        <input type="submit" value="SEND">
    </form>
    ```
> In directory 5 , we used this form .

---

**In html5 , we have symbolic tags that shows every part of html file(instead of use div for all parts)**
*Example:*
+ header
+ nav
+ aside
    + section
    + section
    + section
+ main
    + article
    + article
    + article
+ footer

> In directory 6&gt;index.html , we used these tags .