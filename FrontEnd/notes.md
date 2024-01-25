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
| <p></p>   | Used for defining paragraphs.                 |
| <b></b>   | Represents bold text.                         |
| <h1></h1> | Heading. There are 6 different heading levels |

## HTML Boilerplate

html

<!DOCTYPE html>   represents Document Type with Html updated version(HTML 5)
<html lang="en">    Root Element
	<head>          Metadata
		<meta charset="UTF-8" />
		<meta name="viewport" content="width=device-width, initial-scale=1.0" />
		<title>Document</title>
	</head>
	<body></body>   all the displaying informations
</html>

In Head Tag all the additional informations which are not displayed on the browser/website. Metadata is Data about Data.

![Herarchial](<Screenshot 2024-01-18 225830.png>)

## Attributes

Har element ko hum ek additional property de skte hain like in image element we can give width size as attributes.

Attributes are used to provide additional information about an element.

Syntax of attributes : <tag attribute="value">Content</tag>

id access in css by # and class by .
id is unique whereas class is non unique.

! is emmet abbrevation which is a html plugin.
heading-h1 to h6
h1-biggest; h6-smallest
only 1 h1 tag used in websites. h2 can be multiple.
