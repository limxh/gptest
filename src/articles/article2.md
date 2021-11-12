## Welcome to Maple Publish

## A Quick guide to Markdown
| Date        | Authors: John Doe    | <Contact@example.com>       |

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

### Unordered List item with number
If you need to start an unordered list item with a number followed by a period, you can use a backslash (\\) to escape the period.

| Markdown | Rendered output |
| ----------- | ----------- |
| \- 2000\. The year of dragon. <br> \- 2012\. The year of dragon as well. <br>  |  <ul><li>2000. The year of dragon.</li><li>2012. The year of dragon as well.</li></ul> |

### Adding elements in list

To add another element in a list while preserving the continuity of the list, indent the element four spaces or one tab.

````
* This is the first list item.
* Here's the second list item.

    I need to add another paragraph below the second list item.

* And here's the third list item.
````

[Home Page](../../index.md)
<div style="text-align: right"><a href="../../index.md" >Next Chapter</a> </div>