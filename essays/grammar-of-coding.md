---
layout: essay
type: essay
title: The Grammar Rules of Coding
date: 2020-09-24
labels:
  - Software Engineering
  - Coding Standards
---

## **Using the same "grammar" that the majority follows**

Whenever you are coding something, especially as a beginner, it is one thing to code up a cool to-do list, however coding is another thing when it comes to writing maintainable and scalable code. I think that writing maintainable and scalable code is very important, almost more so than the goal of building the project out. If you are new to coding standards, you might be asking what maintainable and scalable means when it comes to coding. For starters, think of it as following the English grammar rules.

### **Write clean code like it's zero emission**

Writing code that is maintainable and scalable means writing code that someone else can read and make changes to with ease. From my own personal experience, I always try to write code that reads as close to English as possible. This means giving meaningful names to my variables and writing each operation like it is math or like it is symbols that represent English words. By doing so, if someone were to read my code, they could and should be able to read it like English, as if they are reading a book. So far, this covers the basis of maintainable code.

Next up is writing scalable code. However, there are some parts to writing scalable code that are beyond the scope of this topic of coding standards. Nonetheless, writing scalable code means either you or someone else can exmaine the code and make necessary updates efficiently without any high risk of breaking the entire project or product. Part of that is making sure you follow a general standard of where to place things like curly braces and parentheses, and how much indentation is needed for each line of code. For example, let's take a look at this piece of code taken from my [Grub Bot](https://github.com/jackiewong99/grub-bot) project:

Which one looks more maintainable and scalable?

```javascript
1 function collectPosition(position) {
2   COORDS['latitude'] = position.coords.latitude;
3   COORDS['longitude'] = position.coords.longitude;
4 }
```

Maybe this one?

```javascript
1 function collectLatitudeLongitude(num) {
2 COORDS['sideways'] = num.coords.latitude;
3 COORDS['vertical'] = num.coords.longitude;
4
5 }
```

If you were thinking that the first option is more maintainable and scalable, then you are absolutely correct! The first code block is much more well written because it follows the general coding standards of proper indentation, spacing and naming of variable names. Now let's compare the two code blocks.

First off, we will address the elephant in the room, and that is the indentation style between the two code blocks. The top code block has the proper indentation because it gives context that the code between the curly braces only belong to the scope of that function. Now in line 1, the function name in the top code block gives the same meaning as "collectLatitudeLongitude" in the second code block but in a much more concise form. Then the parameter named "position" gives more context than saying "num" as it tells the developer that we are collecting a position rather than just a number. You can think of this like telling someone, "I saw a thing." _versus_ "I saw a dog."

Next up, in lines 2 and 3, the top code block says "latitude" and "longitude", which once again gives more context and meaning to the lines of code rather than just saying that you are assigning to the "sideways" coordinate and "vertical" coordinate. Lastly, the assigned value in the top code block says "position.coords.latitude" and "position.coords.longitude" which I will say like a broken record that it gives more context and meaning than "num.coords.latitude" and "num.coords.longitude". The final nitpick between the two code blocks is that the second one has an unnecessary empty line before the closing curly brace which is taking up more space with no purpose. To sum up the comparison between the two code blocks, the top one has the more pleasing indentation styling and the naming convention is concise yet it gives more context and meaning than the code in the second code block.

Putting this all together, the top code block fulfills the qualities of maintainable and scalable code. If another person were to look at that piece of code, they would only have to read it once and they will understand what the code is trying to do. After that, the person will be able to easily expand on that code, make changes, or use the function for another purpose. Whereas in the second code block, the person will end up having thoughts of why I named a variable "sideways" in the back of their head for the rest of the day. This all explains why I think that coding standards are great and an important part of building any project as it allows all developers to maintain and scale code efficiently. Simply put, you can think of coding standards as to how people keep their rooms organized and tidy.
