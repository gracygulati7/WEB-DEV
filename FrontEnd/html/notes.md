# Web Development

Interconnected network of computers around the world -> Internet

Client ki request ISP(Internet Service Provider) then it goes DNS(address book digital)(it has IP address) send to ISP to Client


## Website

There are 2 types of websites: Static & Dynamic.

| Static                                | Dynamic                                          |
| ------------------------------------- | ------------------------------------------------ |
| whose data is not controlled by user  | whose data's control is in user and client hands |
| It's like a visiting card             | Like Youtube                                     |
| To add webpage in this u need to code | Here u don't                                     |

## How a Website Works

Take Website as a human body where skeleton (HTML) who creates Structure of any website. Muscle , Skin Hair (CSS) defines look/style of website. The body cannot do any functionality so we have brain(JavaScript). In this Brain there is no memory/storage because HTML, CSS and JavaScript are installed in our browser.

For this we use database / server. For the recognition of body we give every website a unique name aka domain name.

User Side:
When we call a website by domain name. Then domain name will locate his server then your request will be given to server then your content will be given to your web browser. Then your browser will read content (Html,CSS, Java Script)

Website Builders are websites which are made without coding.

## HTML

Hyper Text Markup Language

Tags
Component used to design the structure of websites. Acts like a container for content.

Markup Language:
is a language in which we give instructions to browser with the tags.

HTML Elements:
everything from start tag to end tag. Website ke andar maine kuch display krana hai toh we need elements and for elements we need tags.

Nested Elements:
Nesting means kisi element ke andar dusra element use karna like we use h1 tag in body tag. Isse hum element ki properties ko mix kr skte hain.

![!\[Html Elements , Tags And Content\](<Screenshot 2024-01-18 213023.png>)](image.png)

## Tags

| Tags        | Description                                   |
| ----------- | --------------------------------------------- |
| `<p></p>`   | Used for defining paragraphs.                 |
| `<b></b>`   | Represents bold text.                         |
| `<h1></h1>` | Heading. There are 6 different heading levels |

`<p>` if we want spaces as we write to be displayed in this tag then use `<pre>` instead of `<p>`. <br>

## HTML Boilerplate

html

```
<!DOCTYPE html>   represents Document Type with Html updated version(HTML 5)
<html lang="en">    Root Element
	<head>          Metadata
		<meta charset="UTF-8" />
		<meta name="viewport" content="width=device-width, initial-scale=1.0" />
		<title>Document</title>
	</head>
	<body></body>   all the displaying informations
</html>
```

In Head Tag all the additional informations which are not displayed on the browser/website. Metadata is Data about Data.


## Attributes

Har element ko hum ek additional property de skte hain like in image element we can give width size as attributes.

Attributes are used to provide additional information about an element.
Attributes are always specified in the start tag
Attributes usually come in name/value pairs like: name="value"

Syntax of attributes : `<tag attribute="value">Content</tag>`

id access in css by # and class by .
id is unique whereas class is non unique.

! is emmet abbrevation which is a html plugin.
heading-h1 to h6
h1-biggest; h6-smallest
only 1 h1 tag used in websites. h2 can be multiple.

-> in img tag there is an alt attribute.
The required alt attribute for the `<img>` tag specifies an alternate text for an image, if the image for some reason cannot be displayed. This can be due to a slow connection, or an error in the src attribute, or if the user uses a screen reader.

# semantic markup

    it is markup that relates to meaning of content
    two types of tags : semantic and non semantic.
     non semantic tags ko dekhke pta hi nhi lgta content kya hai
     semantic tag egs: h1,p,img
     non semantic tags: div,span
     all websites use SEMANTIC TAGS
      need of semantic tags-
     1. code meaningful bn jata hai, layout-> structured bn jata hai
     2. seo friendly bn jati h website (search engine optimization) means website rank wise achi hogi
     3. readable bnata hai humari website + screen readers performs better
     4. user experience improve hojata hai

**major tags used in semantic markup:**

1. header
2. main tag
3. footer
4. nav
5. article
6. section
7. aside

current webpage pe rehna is anchor tag whereas dusre web page pe jana is nav tag.

# html entities

-> its a piece of text/string what begins with an "&" and ends with a ";". <br>
-> for space it is `&nbsp;` (non breaking space). <br>
-> for < sign it is `&lt;` for > sign it is `&gt;` <br>
-> used to display reserved characters (which would otherwise be interpreted as html code) and invisible characters (like nbsp) <br>
-> can also be used in place of characters that are difficult to type with standard keyboard like a heart `(&hearts;)` <br>
-> browser interprets them & renders corect character.(correct output produced by browsers based on their characters present) <br>

`&quot;` for quotes

| Character | Entity | Note                                       |
| --------- | ------ | ------------------------------------------ |
| &         | amp    | Interpreted as the beginning of an entity  |
|           |        | or character reference.                    |
| <         | lt     | Interpreted as the beginning of a tag      |
| >         | gt     | Interpreted as the ending of a tag         |
| "         | quot   | Interpreted as the beginning and end of an |
|           |        | attribute's value.                         |
| &nbsp;    | nbsp   | Interpreted as the non-breaking space.     |
| –         | ndash  | Interpreted as the en dash                 |
|           |        | (half the width of an em unit).            |
| —         | mdash  | Interpreted as the em dash                 |
|           |        | (equal to the width of an "m" character).  |
| ©         | copy   | Interpreted as the copyright sign.         |
| ®         | reg    | Interpreted as the registered sign.        |
| ™         | trade  | Interpreted as the trademark sign.         |
| ≈         | asymp  | Interpreted as the almost equal to sign.   |
| ≠         | ne     | Interpreted as the not equal to sign.      |
| £         | pound  | Interpreted as the pound symbol.           |
| €         | euro   | Interpreted as the euro symbol.            |
| °         | deg    | Interpreted as the degree symbol.          |

use & in front of entity and ; in the end.

->all entities have a character code associated to them as well. <br>
->all entities have a uni code on mdn html and if we want to use them in html file then we need to convert the uni code to decimal and then use it with &# at the starting. <br>
syntax: &#decimalcode

# Emmet:

-> set of related plugins used by developers. <br>
-> visit emmet.io <br>
_Representation:_ <br>  
-> 1. child: > <br>
syntax: parent>child <br>
eg: if you want div inside p u can write p>div it will be shown as: <br>

```
<p>
    <div>
    </div>
</p>
```

-> 2. sibling: + <br>
syntax: parent>child1+child2 <br>
eg: div and img siblings (p>div+img) <br>

```
<p>
    <div></div>
    <img>
</p>
```

-> 3.Multiplication: _ <br>
if u want a tag to be prined multiple times u can just add _ then the no. of times u want it to be printed. <br>
eg : div\*5 will produce output as: <br>

```
      <div></div>
      <div></div>
      <div></div>
      <div></div>
      <div></div>
```

-> 4. boiler plate code: !
gives basic code of html file.

# HTML5 <br>

-> means new features(upgrades) <br>
-> other things/features that are not part of html (eg: javascript api)

**HOW IT WORKS?** <br>
html standard: <br>
-> its a document that tells browser how html should work.<br>
-> also called as livig standard. (gets updated with time)

# TABLES <br>

-> tables are used to represent real life table data. <br>
-> Attributes: Rows and Columns. <br>

**semantics in table** <br>

```
<thead> -> to wrap table header
<tbody> -> to wrap table body
<tfoot> -> to wrap table footer
```

**table attributes** <br>
`colspan and rowspan attributes:` <br>
span: ek cell kitna area occupy kr rha h table k andr <br>
by default, ek cell table k andr 1 row and 1 col ka area occupy kr rha hota hai <br>
we use these attributes when we want cell to occupy more rows and col than 1 <br>
![alt text](image-1.png)

# style attribute <br>

-> The style attribute is used to add styles to an element, such as color, font, size, and more. <br>

# lang attribute <br>

-> You should always include the lang attribute inside the `<html>` tag, to declare the language of the Web page. <br>
-> This is meant to assist search engines and browsers. <br>

```
<!DOCTYPE html>
<html lang="en">
<body>
...
</body>
</html>
```

# forms <br>

-> they are used to collect data from the user. <br>
**attributes** <br>
-> action attribute is used to define what action needs to be performed when a form is submitted or where the form data should be sent. <br>

```
syntax: <br>
<form action="/action.php">
<form action="/action">
```

**form elements** <br>

1. input element : <br>
   -> used to create multiple form controls. <br>
   -> there are multiple type of inputs that can be created using type attributes. <br>
   -> it is a single tag. no closing tag is required. <br>
   -> it has another element in it ie type element that tells the type of input. <br>
   ![alt text](image3.png) <br>
   -> next attribute of input element is placeholder. <br>
   -> it is the light text shown before we enter the actual input. <br>

2. label: <br>
-> it represents a caption for an item in a user interface. <br>
-> more formally we will use label and input differently and form a connection btw them using for attribute in label and id attribute in input. <br>
-> id is a unique name (attribute) associated with any element. <br>
```
syntax: <label for="id">Label</label>
<input type="type_name" id="id_name" placeholder="enter text">
```
-> label k andr ka for ki value and input k andr k id ki value should be the same to build a connection between the two. <br>

3. button: <br>
-> iska default behaviour in form is to submit the data to the server or url which is mentioned in action attribute of button. <br>
-> if its written in form then we would have to define its behaviour. <br> <br>
![alt text](button.png)
<br>
-> Submit pe click krne se sari info form ki submit ho jayegi <br>
-> Reset pe click krne se form ke saare fields empty ho jaenge <br>
-> Button pe click krne se action jo hamne form tag ke sath bhara hai vo ho jaega <br>
-> Button pe click krne se koi action nhi hoga if its outside the form unless u mention the action with it that what does tht button needs to do <br>
-> input element ki form mein button create kr skte hai <br>
syntax: ``` <input type="submit" value="click me"> ``` <br>

4. Name attribute: <br>
-> name of the form control. submitted with the form as a part of name/value pair. <br>
->  it is there to know at the backend that what type of info or what info was entered in the input box. so that we can access it at backend. <br>
-> name/val pair mein name is the name i gave to my input box in code and value is the value entered by yser in the input box. <br>

5. checkbox: <br>
-> input type mein agr checkbox dedu toh checkbox create ho jata hai <br>
```
syntax: 
<input type="checkbox" name="age" id="age" checked >
<label for="age">I am 18+</label>
```
-> if i write checked then by default the checkbox appears already ticked , i can untick it also. <br>
-> if i dont write checked then it will appear as unchecked and i can tick it again <br>
-> if i submit the form with ticked checkbox then the information gets submitted in action url as name=on (name is the name that we gave to our input element by which it can be accessed at backend) <br>
![](checkbox_on.png)
-> if i submit the form with unticked checkbox then nothing gets passed on to the action url. <br>
![](checkbox_off.png)

6. radio button: <br>
-> only one radio button can be selected at a time whereas multiple chcekboxes can be selected at once. <br>
```
syntax: 
<input type="radio" name="fruits" id="apple" value="apple">
<label for="apple">Apple</label>
```
-> if name attribute is same only then can i group multiple radio buttons together and then we can only select one radio button as only one value of the name attribute will be sent to the action url. <br>
-> here value attribute is used to tell the action url which radio button is selected. <br>
-> like action url also has name-value pairs. <br>
-> so here name is same for all radio buttons but the value that will be passed will be one of the radio buttons and that value will be known only by the value attribute. <br>


7. select element: <br>
-> dropdowns create krne ke liye we use select element <br>
-> selected attribute is used to pre select any element <br>
```
syntax:
<select name="profession" id="profession">
<option value="student">Student</option>
<option value="dev">Developer</option>
</select>
```  
![alt text](dropdown.png)

8. range input: <br>
-> to select any value in range. <br>
```
syntax:
<label for="vol">Select Volume Level</label>
<input type="range" id="vol" min="0" max="100" name="vol" step="10" value="70">
```
-> here ange starts from mn=0 and max=100 and it increases in step size like if i just move my range by 1 forward so it will be of 10 value. <br>
-> step attribute is used when i want my data to increase in range in fixed values only. <br>
-> value attribute sets a default value in range when a user just opens a form and it can be changed. <br>

9. text area element: <br>
-> if like we want some feedback in form then this is used.
```
syntax:
<label for="feedback">Please give your feedback:</label>
<textarea id="feedback" name="feedback" rows="5" cols="20" placeholder="write your feedback here"></textarea>
```
-> default size is 2 rows and 10 cols but we can resize it using rows and cols attributes. <br>