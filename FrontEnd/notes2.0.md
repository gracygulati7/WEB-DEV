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

Hyper Text Markup Language and is NOT A CASE SENSITIVE LANGUAGE.

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

| Tags                                                     | Description                                                                                                                                                         |
| -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p></p>                                                | Used for defining paragraphs.                                                                                                                                       |
| <b></b>                                                | Represents bold text.                                                                                                                                               |
| <h1></h1>                                              | Heading. There are 6 different heading levels                                                                                                                       |
| <a href ="Link">Text If Link Not Printed</a>           | Anchor tag is used when after clicking on something we shift to other position. href stands for Hyper Text Reference                                                |
| <img src ="imagename.png" alt="Text other than Image"> | Open Tag. Alt attribute is alternate text                                                                                                                           |
| <ul></ul>                                              | unordered list                                                                                                                                                      |
| <li></li>                                              | List is created by this tag only                                                                                                                                    |
| <ol></ol>                                              | Ordered list                                                                                                                                                        |
| <br>                                                   | br tag is empty tag and open tag also known as for line breaks                                                                                                      |
| Div Element                                            | Container used to hold other HTML element or group elements together and is a block element. He has no functionality of its own                                     |
| Span Element                                           | similar as Div Element ; generic container used to hold other HTML elements or goups together and major difference between Span and Div is : Span is Inline Element |
| <hr>                                                   | Horizontal Line Divider                                                                                                                                             |
| <sup></sup>                                            | Superscript                                                                                                                                                         |
| <sub></sub>                                            | Subscript                                                                                                                                                           |
| <section></section>                                    | Section Tag: Used To create sections of the page                                                                                                                                               |
| <aside></aside>                                        | Aside Tag : Sara Content Side By Side Aega                                                                                                                          |
| <nav></nav>                                            | Navigation Tag                                                                                                                                                      |
| <footer></footer>                                      | Footer Tag                                                                                                                                                          |
| <tr></tr>                                              | Table rows display                                                                                                                                                  |
| <td>/td>                                               | Used to display table data                                                                                                                                          |
| <th></th>                                              | Used to display table heading                                                                                                                                       |
| <pre>/pre>                                             | Displays as it is with the same level of spaces                                                                                                                     |


## HTML Boilerplate

html
<!doctype html> represents Document Type with Html updated version(HTML 5)
<html lang="en">
	Root Tag
	<head>
		Metadata
		<meta charset="UTF-8" />
		<meta name="viewport" content="width=device-width, initial-scale=1.0" />
		<title>Document</title>
	</head>
	<body></body>
	all the displaying informations
</html>


In Head Tag all the additional informations which are not displayed on the browser/website. Metadata is Data about Data. Emmet abbrivation is a plugin for time saving.

![Herarchial](<Screenshot 2024-01-18 225830.png>)

## Attributes

Har element ko hum ek additional property de skte hain like in image element we can give width size as attributes.

Attributes are used to provide additional information about an element.

Like <html lang="en" > lang is attribute.

Syntax of attributes : <tag attribute="value">Content</tag>

## ID VS Class

ID is unique in the whole document whereas Class is not unique

## List

they are of 2 types:

1. Unordered List
2. Ordered List

## Index html file

Index is a special name which we give to our main file when we are making a big project.

## Difference Between Inline and Block

| INLINE                                                 | BLOCK                             |
| ------------------------------------------------------ | --------------------------------- |
| Takes Necessary width                                  | Takes up full width available     |
| Example multiple cycles can be placed in a single line | you can place one cycle in 1 line |
| Don't Start from New Line                              | Starts from New Line              |
|                                                        | Like Heading Tag takes full line  |

## SEMANTIC TAGS V/S NON-SEMANTIC TAGS

Semantic tags are the one which we can know about them just after veiwing the tag whereas we can not guess in non-semantic ones.

Semantic Example : Like <h1> tag jisko dekh ke ham bata sakte hai ki yeah heading tag hai. All the websites use SEMANTIC MARKUP.

Semantic Markup means hamein meaning se matlab hai. After using Semantic code meaningful ban jata hai i.e structured ban jata hai.

SEO : Search Engine Optimisation. Whenever we go to chrome, it finds semantic tags and seo friendly hone se easily hamari website chrome dikha pata hai. Semantic make our code more readable. isse user experience improve ho jata hai.

--> MAJOR TAGS USED IN SEMANTIC MARKUP

-   Header Tag <header>
-   Main Content <main>
-   Footer Tag <footer>
-   Nav Tag <nav>
-   Section Tag <section>
-   Aside Tag <aside>

They are used once in a website. We can use them more than once but it is incorrect.

## HTML ENTITIES

it's a peice of text/string which begins with & and ends with semicolon(;)

-   for non - breaking space (&nbsp;)
-   for less than symbol (&lt;)
-   for greater than symbol (&gt;)
-   used to display reserved character (which would otherwise be interpreted as html code) and invisible characters like nbsp
-   can be used to display the characters that are difficult to type with a standard keybord like &hearts;
-   browser interprets them & renders correct character (correct output produced by browsers based on their characters present)
-   Quotes Print krane ke liye quot

| Character | Entity | Note                                                                 |
| --------- | ------ | -------------------------------------------------------------------- |
| &         | amp    | Interpreted as the beginning of an entity or character reference.    |
| <         | lt     | Interpreted as the beginning of a tag                                |
| >         | gt     | Interpreted as the ending of a tag                                   |
| "         | quot   | Interpreted as the beginning and end of an attribute's value.        |
| &nbsp;    | nbsp   | Interpreted as the non-breaking space.                               |
| –         | ndash  | Interpreted as the en dash (half the width of an em unit).           |
| —         | mdash  | Interpreted as the em dash (equal to the width of an "m" character). |
| ©        | copy   | Interpreted as the copyright sign.                                   |
| ®        | reg    | Interpreted as the registered sign.                                  |
| ™        | trade  | Interpreted as the trademark sign.                                   |
| ≈         | asymp  | Interpreted as the almost equal to sign.                             |
| ≠         | ne     | Interpreted as the not equal to sign.                                |
| £         | pound  | Interpreted as the pound symbol.                                     |
| €         | euro   | Interpreted as the euro symbol.                                      |
| °         | deg    | Interpreted as the degree symbol.                                    |

Use & in front of entity and ; in the end. All the entities have a character code to them as well. All entities have a uni code and if we want to use them in html file then we need to convert the uni code to decimal and then use it with &# in the starting

SYNTAX: &#decimalcode

## Emmet

It is not directly to html or development. It is set of related plugins used by developers. Emmet.io is essential toolkit for developers.

--> Child/Parent Relation
<br>
Parent is that entity jo upar aata hai hamse.

-   p>div creates a p "Parent Tag" with a child tag "Div"
-   div\*5 creates tag div tag 5 times.

--> Siblings
<br>
Jo same level pe aate hain

Example:

html
<p>
    <div></div>
    <img>
</p>


Here, div and img tag are siblings.
<br>
"+" is used to create sibling tags.

--> Multiplication
<br>
Creates tag multiple time. div\*5 means tag will be repeated 5 times.

## HTML 5

-   Means New Features
-   other things/features that are not a part of html like javascript api

*HOW IT WORKS?*
<br>
html standard-> it is a document that tells browser how html should work. It is also called a living Standard (gets updated by time).

## Tables

Used to represent real life table data.
<br>
Attributes: Row & Column.

Table Header is jo sare table ka information dega

