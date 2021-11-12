## Welcome to Maple Publish

## A Quick guide to Markdown
| Date: "Last compiled on `r format(Sys.time(), '%d %B, %Y')`"        | Authors: John Doe    | <Contact@example.com>       |

___


Nearly all Markdown applications support the basic syntax outlined in John Gruber’s original design document. There are minor variations and discrepancies between Markdown processors.

## Headings

Add number signs (#) in front of a word or phrase to create a heading. The number of number signs corresponds to the heading level. For example, to create a heading level four (\<h4>), use four number signs (e.g., #### My Level Four Header).

Alternatively, on the line below the text, add any number of == characters for heading level 1 or -- characters for heading level 2.

| Markdown | Rendered output |
| ----------- | ----------- |
| \# Heading Level 1 |  <h1>Heading Level 1</h1> |
| \## Heading Level 2 |  <h2>Heading Level 2</h2> |
| \### Heading Level 3 |  <h3>Heading Level 3</h3> |
|  Heading Level 1 <br> =========== |  <h1>Heading Level 3</h1> |
|  Heading Level 2 <br> ------------------ |  <h2>Heading Level 3</h2> |

## Paragraphs and Line breaks

To create paragraphs, use a blank line to separate one or more lines of text.

To create a line break (\<br>), end a line with two or more spaces, and then type return.

| Markdown | Rendered output |
| ----------- | ----------- |
| Markdown is very simple. <br> You can even incorporate html style in it.|  Markdown is very simple. <br> You can even incorporate html style in it. |

## Emphasis

Emphasis could be added by making text bold or italic.

### **Bold**

To bold text, add two asterisks or underscores before and after a word or phrase. To bold the middle of a word for emphasis, add two asterisks without spaces around the letters.

### *Italic*

To italicize text, add one asterisk or underscore before and after a word or phrase. To italicize the middle of a word for emphasis, add one asterisk without spaces around the letters.

### ***Bold and Italic***

To emphasize text with bold and italics at the same time, add three asterisks or underscores before and after a word or phrase. To bold and italicize the middle of a word for emphasis, add three asterisks without spaces around the letters.

| Markdown | Rendered output |
| ----------- | ----------- |
| This is \*\*bold**|  This is **bold** |
| This is \_\_bold__|  This is __bold__ |
| This is \*italic*|  This is *italic* |
| This is \_italic_|  This is *italic* |
| This is \*\*\*bold and italic***|  This is ***bold and italic*** |
| This is \_\_\_bold and italic___|  This is ***bold and italic*** |
| This is \*\*\_bold and italic_**|  This is **_bold and italic_** |
| This is \_\*\*bold and italic**_|  This is _**bold and italic**_ |

## Blockquotes

To create a blockquote, add a > in front of a paragraph.

````
> Vision is not what your eyes see, but an image your brain comprehends
````

The rendered output:

> Vision is not what your eyes see, but an image your brain comprehends

## Blockquotes with multiple paragraphs

Blockquotes can contain multiple paragraphs. Add a > on the blank lines between the paragraphs

````
> Vision is not what your eyes see, but an image your brain comprehends
>
> Life comes at a cost. Wouldn’t it be arrogant to die before you’ve repaid that debt?
````

The rendered output:

> Vision is not what your eyes see, but an image your brain comprehends
>
> Life comes at a cost. Wouldn’t it be arrogant to die before you’ve repaid that debt?

## Nested Blockquotes

Blockquotes can be nested. Add a >> in front of the paragraph you want to nest.

````
> Vision is not what your eyes see, but an image your brain comprehends
>
>> Life comes at a cost. Wouldn’t it be arrogant to die before you’ve repaid that debt?
````

The rendered output:

> Vision is not what your eyes see, but an image your brain comprehends
>
>> Life comes at a cost. Wouldn’t it be arrogant to die before you’ve repaid that debt?

## Blockquotes with other elements

Blockquotes can contain other Markdown formatted elements. Not all elements can be used — you’ll need to experiment to see which ones work.

````
> ## Best quotes you need
> - Vision is not what your eyes see, but an image your brain comprehends
> - Life comes at a cost. Wouldn’t it be arrogant to die before you’ve repaid that debt?
>
> **Life** is not a ***game of luck***. *If you wanna win, work hard.*
````

The rendered output:

> ## Best quotes you need
> - Vision is not what your eyes see, but an image your brain comprehends
> - Life comes at a cost. Wouldn’t it be arrogant to die before you’ve repaid that debt?
>
> **Life** is not a ***game of luck***. *If you wanna win, work hard.*

## Lists

You can create ordered and unordered lists.

### Ordered List

To create an ordered list, add line items with numbers followed by periods. The numbers don’t have to be in numerical order, but the list should start with the number one.

| Markdown | Rendered output |
| ----------- | ----------- |
| 1. First <br> 2. Second <br> 3. Third <br> 4. Fourth |  1. First <br> 2. Second <br> 2. Third <br> 2. Fourth |
| 2. First <br> 2. Second <br> 3. Third <br> 4. Fourth |  1. First <br> 2. Second <br> 3. Third <br> 4. Fourth |
| 3. First <br> 6. Second <br> 5. Third <br> 8. Fourth |  1. First <br> 2. Second <br> 3. Third <br> 4. Fourth |
| 1. First <br> 2. Second <br> 3. Third <br> &emsp; 1. Indented item <br> &emsp; 2. Indented item <br> 4. Fourth |  1. First <br> 2. Second <br> 3. Third <br> &emsp; 1. Indented item <br> &emsp; 2. Indented item <br> 4. Fourth |

### Unordered List

To create an unordered list, add dashes (-), asterisks (*), or plus signs (+) in front of line items. Indent one or more items to create a nested list.

| Markdown | Rendered output |
| ----------- | ----------- |
| \- First <br> \- Second <br> \- Third <br> \- Fourth |  <ul><li>First item</li><li>Second item</li><li>Third item</li><li>Fourth item</li></ul> |
| \* First <br> \* Second <br> \* Third <br> \* Fourth |  <ul><li>First item</li><li>Second item</li><li>Third item</li><li>Fourth item</li></ul> |
| \+ First <br> \+ Second <br> \+ Third <br> \+ Fourth |  <ul><li>First item</li><li>Second item</li><li>Third item</li><li>Fourth item</li></ul> |
| \- First <br> \- Second <br> \- Third <br> &emsp; \- Indented item <br> &emsp; \- Indented item <br> \- Fourth |  <ul><li>First item</li><li>Second item</li><li>Third item<ul><li>Indented item</li><li>Indented item</li></ul></li><li>Fourth item</li></ul> |

The rendered output:
<ul>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
  <li>Fourth item</li>
</ul>


### Unordered List item with number
If you need to start an unordered list item with a number followed by a period, you can use a backslash (\\) to escape the period.

| Markdown | Rendered output |
| ----------- | ----------- |
| \- 2000\. The year of dragon. <br> \- 2012\. The year of dragon as well. <br>  |  <ul><li>2000. The year of dragon.</li><li>2012. The year of dragon as well.</li></ul> |

### Adding elements in list

To add another element in a list while preserving the continuity of the list, indent the element four spaces or one tab.

````
### Example list with multiple types of elements added
* This is the first list item.
* This is how you add paragraph.

    I need to add another paragraph below the second list item.

* This is how you add blockquote.
  
    > A blockquote would look great below the second list item.

* This is how you add code blocks. Code blocks are normally indented four spaces or one tab. When they’re in a list, indent them eight spaces or two tabs.

        <html>
          <head>
            <title>Test</title>
          </head>

* This is how you add images

    ![logo](/src/images/images.jfif)

````

The rendered output:

### Example list with multiple types of elements added
* This is the first list item.
* This is how you add paragraph.

    I need to add another paragraph below the second list item.

* This is how you add blockquote.
  
    > A blockquote would look great below the second list item.

* This is how you add code blocks. Code blocks are normally indented four spaces or one tab. When they’re in a list, indent them eight spaces or two tabs.

        <html>
          <head>
            <title>Test</title>
          </head>

* This is how you add images

    ![logo](../images/images.jfif)


## Code

To denote a word or phrase as code, enclose it in backticks (`).

## Escaping Backtick

If the word or phrase you want to denote as code includes one or more backticks, you can escape it by enclosing the word or phrase in double backticks (``).

| Markdown | Rendered output |
| ----------- | ----------- |
| Code example: At the command prompt, type \`nano\`.  |  Code example: At the command prompt, type `nano`. |
| Escaping backtick example: \`\`Use \`code\` in your Markdown file.\`\`.  |  Escaping backtick example: ``Use `code` in your Markdown file.``. |

## Code Blocks

To create code blocks, indent every line of the block by at least four spaces or one tab.

````
    <html>
      <head>
      </head>
    </html>
````

The rendered output:

    <html>
      <head>
      </head>
    </html>

## Horizontal Rules

To create a horizontal rule, use three or more asterisks (***), dashes (---), or underscores (___) on a line by themselves.

````
***

---

_________________
````

The rendered output:

***

---

_________________

## Links

To create a link, enclose the link text in brackets (e.g., [Duck Duck Go]) and then follow it immediately with the URL in parentheses (e.g., (`https://google.com`)).

````
My favorite search engine is [Google](https://google.com "The best search engine").
````

The rendered output:

My favorite search engine is [Google](https://google.com "The best search engine").


## URLs and emails

To quickly turn a URL or email address into a link, enclose it in angle brackets.

````
<https://www.markdownguide.org>

<fake@example.com>
````

The rendered output:

<https://www.markdownguide.org>

<fake@example.com>

## Images

To add an image, add an exclamation mark (!), followed by alt text in brackets, and the path or URL to the image asset in parentheses. You can optionally add a title after the URL in the parentheses.

````
![logo](../images/images.jfif)
````

The rendered output:

![logo](../images/images.jfif)

## Linking images

To add a link to an image, enclose the Markdown for the image in brackets, and then add the link in parentheses.

````
[![logo](../images/images.jfif)](https://www.macmillandictionary.com/dictionary/british/maple)
````

The rendered output:

[![logo](../images/images.jfif)](https://www.macmillandictionary.com/dictionary/british/maple)

## Escaping characters

Escaping Characters
To display a literal character that would otherwise be used to format text in a Markdown document, add a backslash (\\) in front of the character.

The characters you can escape includes \\, \`, \*, \_, \{\}, \[\], \<\>, \(\), \#, \+, \-, \., \!, \|.

## HTML

Many Markdown applications allow you to use HTML tags in Markdown-formatted text. This is helpful if you prefer certain HTML tags to Markdown syntax. For example, some people find it easier to use HTML tags for images. Using HTML is also helpful when you need to change the attributes of an element, like specifying the color of text or changing the width of an image.

To use HTML, place the tags in the text of your Markdown-formatted file.

## Video

<video width="320" height="240" controls>
  <source src="../video/vid01.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

## Further information regarding markdown syntax

For more information about markdown syntax, you could visit [Markdown Guide](https://www.markdownguide.org/ "Markdown guide").

[Home Page](../../index.md)
<div style="text-align: right"><a href="../../index.md" >Next Chapter</a> </div>