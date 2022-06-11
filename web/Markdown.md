---
layout: default
title: Markdown 
---

<h1>Markdown</h1>

Markdown is a **markup language**.

A **Markdown application** converts Markdown-formatted text to HTML.

[Dillinger](https://dillinger.io/) is an online Markdown editor with preview capability.

<hr>
## Basic Markdown Syntax

# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6

Alt Heading 1
==================

Alt Heading 2
--------


<hr>
## Best Practices
- Always put a space after the #<br>
Always put a blank line before and after the heading.

- Use a blank line between texts to create a paragraph.

- Use 2+ spaces and a <return> to create a line break.<br>
Or use &lt;br&gt; to create a line break.

<hr>
## Italic, Bold, and Code
*itatic*<br>
**bold**<br>
***bold and italic***

`code`

Code blocks are indented 4 space or 1 tab.
If the code block is inside a list, then indent by 8 spaces or 2 tabs.

    if True:
        print("Hello, World!")

<hr>
## Blockquotes


>
> ## Header
>
> Make sure to put blank lines before and after blockquotes.
>
>> Nested blockquotes
>

<hr>

## Lists

### Ordered Lists
1. first
2. second
3. third

### Unordered List
- first

    This is indented by 1 tab or 4 spaces.

- second
    - nested item
- third

    > This is an indented blockquote.

Can use -, +, or * as the symbol for a list item.



<hr>
## Extended Markdown Syntax
(Not available everywhere)

==highlight==

<mark>highlight<mark>

#### Fenced Code Block with Syntax Highlighting

```css
p.invert {
  background-color: blue;
  color: white;
}
```

or 

~~~css
p.invert {
  background-color: blue;
  color: white;
}
~~~

<img class="large_picture" src="/images/Markdown.png" />
