---
layout: essay
type: essay
title: Not So Quick Styling
date: 2020-10-08
labels:
  - Software Engineering
  - UI Frameworks
  - Styling
---

## **Styling made easy through UI Frameworks but no so quick to use**

As the minutes go by, and the sun rises and sets cyclically, I find myself learning a UI framework called [Semantic UI](https://semantic-ui.com/) for the past week. I must say, _Semantic UI_ is definitely a great alternative to creating styles from scratch. This is especially great for people who are not looking to be front-end developers and just need a quick touch up on the design of their projects. However, from my experience I did not enjoy using _Semantic UI_ as much as I thought I would, felt that I could have achieved the same results with raw HTML and CSS, and think that [Twitter Bootstrap](https://getbootstrap.com/) is a better UI framework.

First off, I had to spend a good amount of time to learn the basics of _Semantic UI_ and then built up frustration whenever I wanted to style an element with specific styling. Compared to other UI frameworks like _Twitter Bootstrap_, _Semantic UI_'s philosophy and structure of their framework is all about using the "natural language." For those who are unsure about what it means to use the "natural language" when it comes to coding something, this means that the code and structure of typing reads like a regular English sentence. To _Semantic UI_'s credit, they were definitely able to achieve that goal of making a "natural language" UI framework. However, the main gripe I have with this framework using the "natural language" is that the keywords become so simple to the point where things can get messy. For example, when you want to style an element, sometimes an element will require the "ui" class and in other times an element does not need the "ui" class and only needs the "fitted item" classes. This can be very confusing for people who are just beginning to learn web development and UI frameworks. I think that this is where _Semantic UI_ oversimplified styling and split up styling into too many small pieces to a point where remembering the terminology becomes a headache.

Secondly, I felt that I could achieve the same results with raw HTML and CSS when I was experimenting with _Semantic UI_ this past week. For some backgound, up to this point I have now experienced using _Semantic UI_ and _Twitter Bootstrap_. When I was creating a few simple web pages and replica projects, I once again found it very frustrating whenever I wanted to create my own bespoke styles and override certain built-in styles from _Semantic UI_. Notice that I said "once again," this is because that phrase ties into my overall opinion on UI frameworks. I understand that I can easily override styles by referencing the _Semantic UI_ class names in my _CSS_ file, however through experience and research, I found this to be bad practice for larger projects and a bad habit to keep in general. This is because if I were to build a larger project rather than a simple functionless web page, targeting the UI framework's class names directly will cause problems like applying the style to many other elements that are also using those class names but are meant to have different styles. That problem can also lead to confusion if I try to track the styling for certain elements and try to read the style sheet another day.

Lastly, if I had a choice, I would choose _Twitter Bootstrap_ over _Semantic UI_. Even though _Twitter Bootstrap_'s class name structure does not read like the "natural language," the naming scheme is much more clean and organized in comparison to _Semantic UI_'s naming scheme. The main factor that makes me prefer _Twitter Bootstrap_ is that there is no need to remember which situations require me to include the "ui" class name. Furthermore, if I ever needed a style from _Twitter Bootstrap_, all I need to do is add the class name to the list of classes. For example, if you want to make a container of elements, all you have to do is give a div element the class "container," whereas in _Semantic UI_, you would have to remember that creating a container requires you to give the classes "ui container." I also like that _Twitter Bootstrap_ allows you to essentially edit styles in the class attribute. For instance, say you have a container:

```html
<div class="container">Hello</div>
```

Then you decide that this container should have a width of 75%. All you have to do is add the class "w-75" where _w_ is the class for changing the width of an element and _75_ represents the percentage value:

```html
<div class="container w-75">Hello</div>
```

This small feature about _Twitter Bootstrap_ is really great for styling elements on the fly without needing to touch any CSS file. Some people may say that this naming scheme like naming the class for width with just the letter, _w_, is vague and confusing, however I think that this is great organization and structure for adding classes to an element. Instead, I think that _Semantic UI_'s naming scheme is too simple, to a point where adding many classes can lead to confusion when revisiting the code.

Overall, in my opinion, I did not enjoy using _Semantic UI_, feel that you are better off using raw HTML and CSS, and think that _Twitter Bootstrap_ is a better UI framework. However, this is not to say that I think _Semantic UI_ is a bad UI framework by any means. I still think that _Semantic UI_ is purposeful and it is clearly good as people stil use it. However, I found that the schema of _Twitter Bootstrap_ is much more efficient and productive than _Semantic UI_. In the end, I think that UI frameworks is great for those who are not the best at UI design or have a project where styling is not the main purpose, and I very much prefer using raw HTML and CSS to style any project I work on.
