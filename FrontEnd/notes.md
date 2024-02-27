# Web Development

Interconnected network of computers around the world -> Internet

Client ki request ISP(Internet Service Provider) then it goes DNS(address book digital)(it has IP address) send to ISP to Client

![Alt text](<Screenshot 2024-01-18 191252.png>)

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

![Html Elements , Tags And Content](<Screenshot 2024-01-18 213023.png>)

## Tags

| Tags      | Description                                   |
| --------- | --------------------------------------------- |
| `<p></p>`   | Used for defining paragraphs.                 |
| `<b></b>`   | Represents bold text.                         |
| `<h1></h1>` | Heading. There are 6 different heading levels |

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

![Herarchial](<Screenshot 2024-01-18 225830.png>)

## Attributes

Har element ko hum ek additional property de skte hain like in image element we can give width size as attributes.

Attributes are used to provide additional information about an element.

Syntax of attributes : `<tag attribute="value">Content</tag>`

id access in css by # and class by .
id is unique whereas class is non unique.

! is emmet abbrevation which is a html plugin.
heading-h1 to h6
h1-biggest; h6-smallest
only 1 h1 tag used in websites. h2 can be multiple.

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

| Character | Entity   | Note                                            |
|-----------|----------|-------------------------------------------------|
| &         | amp      | Interpreted as the beginning of an entity       |
|           |          | or character reference.                         |
| <         | lt       | Interpreted as the beginning of a tag           |
| >         | gt       | Interpreted as the ending of a tag              |
| "         | quot     | Interpreted as the beginning and end of an      |
|           |          | attribute's value.                              |
| &nbsp;    | nbsp     | Interpreted as the non-breaking space.          |
| –         | ndash    | Interpreted as the en dash                      |
|           |          | (half the width of an em unit).                 |
| —         | mdash    | Interpreted as the em dash                      |
|           |          | (equal to the width of an "m" character).       |
| ©         | copy     | Interpreted as the copyright sign.              |
| ®         | reg      | Interpreted as the registered sign.             |
| ™         | trade    | Interpreted as the trademark sign.              |
| ≈         | asymp    | Interpreted as the almost equal to sign.        |
| ≠         | ne       | Interpreted as the not equal to sign.           |
| £         | pound    | Interpreted as the pound symbol.                |
| €         | euro     | Interpreted as the euro symbol.                 |
| °         | deg      | Interpreted as the degree symbol.               |

use & in front of entity and ; in the end.

->all entities have a character code associated to them as well. <br>
->all entities have a uni code on mdn html and if we want to use them in html file then we need to convert the uni code to decimal and then use it with &# at the starting. <br>
syntax: &#decimalcode


# Emmet:
-> set of related plugins used by developers. <br>
-> visit emmet.io <br>
*Representation:* <br>  
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

-> 3.Multiplication: * <br>
if u want a tag to be prined multiple times u can just add * then the no. of times u want it to be printed. <br>
eg : div*5 will produce output as: <br>
     
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


