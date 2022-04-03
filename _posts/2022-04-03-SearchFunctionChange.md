---
title: New Search Function - GlpiTools
categories:
    - Glpi
tags:
    - GlpiTools
---

Long story short 😀 Let's begin !

First, go to the doc which describing the Search Function  
[Search-GlpiToolsItems](https://www.wpietrzak.pl/glpi/Search-GlpiToolsItems/)  

Now you are able to put more filtering on a search, you can link with the operators like **AND**  
But the better way to descibe it, is to have a real example  
Here is command which gets the computers  
**Search-GlpiToolsItems -SearchFor Computer -SearchType contains, contains -SearchField 1, 40 -SearchValue c, virtual -SearchLink AND**  

And now:  
**SearchFor** here we put what we want to search  
**SearchType** here you can specify a type of a search, you can choose between values like **contains** **equals** and more, you can put here more than one type  
**SearchField** here you need to specify field of a search which you can get from different command, and as well you can put here more than one value  
**SearchValue** put here values that you want to search, you can put more than one  
**SearchLink** here you are able to choose how do you want to link these values, **you have two values for SearchType, SearchField, SearchValue you linking them with one SearchLink**  like in a example  

**This command has backward compatibility so you shoudn't have problems with your scripts after module update, but be aware of this!**  