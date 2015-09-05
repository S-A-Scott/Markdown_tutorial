# Markdown tutorial

* [Markdown Basics](#markdown-basics)
    * [What is Markdown](#what-is-markdown)
    * [Github Flavored Markdown](#github-flavored-markdown)
* [Lesson1 Emphasis and Headers](#lesson1-emphasis-and-headers)
    * [Emphasis](#emphasis)
		* [Italics](#italics)
        * [Bold](#bold)
    * [Headers](#headers)
* [Lesson2 Links](#lesson2-links)
    * [Inline Link](#inline-link)
    * [Reference Link](#reference-link)
* [Lesson3 Images](#lesson3-images)
    * [Inline Image Link](#inline-image-link)
    * [Reference Image Link](#reference-image-link)
* [Lesson4 Lists](#lesson4-lists)
    * [Unordered Lists](#unordered-lists)
    * [Ordered Lists](#ordered-lists)
    * [Nested Lists](#nested-lists)
* [Lesson5 Blockquotes and Paragraphs](#lesson5-blockquotes-and-paragraphs)
    * [Blockquotes](#blockquotes)
    * [Paragraphs](#paragraphs)
        * [Hard Break](#hard-break)
        * [Soft Break](#soft-break)
* [Lesson6 Code](#lesson7-code)
    * [Inline Code](#inline-code)
    * [Code Blocks](#code-blocks)
        * [Syntax highlighting](#syntax-highlighting)


# Markdown Basics


## What is Markdown

[Markdown](http://daringfireball.net/project/markdown) is a way to style text on the web. You control the display of the document; formatting
words as bold or italic, adding images, and creating lists are just a few of the things we can do with
Markdown. Mostly, Markdown is just regular text with a few non-alphabetic characters thrown in, like # or *.

## Github Flavored Markdown

GitHub.com uses its own version of the Markdown syntax that provides an additional set of
useful features, many of which make it easier to work with content on GitHub.com

# Lesson1 Emphasis and Headers

We'll start by learning two basic elements in Markdown: **_Emphasis_** and headers.

## Emphasis

There are two ways to emphasis the text: _italics_ and **bold**.

### Italics

To make a phrase _italic_ in Markdown, you can surround words with an undersocre(_).  
For example, input:
```
_This text will be italic_.
```

will output:  
  _This text will be italic_.

#####NOTE

Where Markdown transforms undersocre(_) into italics, Github Flavored Markdown(GFM) ignores undersocre in words, like
* make_pair
* uninitialized_copy_n

### Bold

Similarly, to make phrase **bold** in Markdown, you can surround words with two asterisks(**).  
For example, input:
```
**This text will be bold**
```

will output:  
  **This text will be bold**

Of course, you can combine italic and bold in the same line.  
For example, input:
```
**_This text will be italics and bold_**
```

will output:  
**_This text will be italics and bold_**

## Headers

You can create a heading by adding one or more hash(#). You place the same number of # makes as the size of the header you want.  
For example, input
```
# Header one
## Header two
### Header three
#### Header four
##### Header five
###### Header six
```

will output:  
# Header one
## Header two
### Header three
#### Header four
##### Header five
###### Header six

# Lesson2 Links

Markdown supports two styles for creating links: inline and reference. With both styles, you use square brackets to delimit the text you want to turn into a link.

## Inline Link

To create an inline link, you warp the link text in brackets([]), and then warp the link in parenthesis( () ).  
For example, to create a hypelink to www.google.com, with a text that says, "GO TO GOOGLE", you write this in Markdown:
```
[GO TO GOOGLE](https://www.google.com)
```

It will turns to:  
[GO TO GOOGLE](https://www.google.com)

#####NOTE

GFW will autolink standard URLs, so if you want to link to a URL(instead of setting link text), you can simply enter the URL and it will be turned into a link to that URL.

## Reference Link

The other link type is reference link. As the name implies, the link is actually a reference to another place in the document. Here's an example:
```
There is [a website for you][1].
There is [another website for you][2].

[1]: https://www.google.com
[2]: https://www.github.com
```

Output:  
There is [a website for you][1].  
There is [another website for you][2].

[1]: https://www.google.com
[2]: https://www.github.com


# Lesson3 Images

Image syntax is very much like link syntax. If you know how to create links in Markdown, you can create images too.

The only difference between two syntax is that an image is prefaced with an exclamation point(!).

Images also have two styles, inline and reference, just like links.

## Inline Image Link

Input:  
```
![alt text](https://octodex.github.com/images/octdrey-catburn.jpg)
```

Output:  
![alt text](https://octodex.github.com/images/octdrey-catburn.jpg)

## Reference Image Link

Input:  
```
![alt text][1]

[1]: https://octodex.github.com/images/octdrey-catburn.jpg
```

Output:  
![alt text][1]

[1]: https://octodex.github.com/images/octdrey-catburn.jpg


# Lesson4 Lists

Markdown supports ordered(numbered) and unordered(bulleted) lists.

## Unordered Lists

To create an unordered list, use asterisks(*), pluses(+), and hyphens(-) --interchangably-- as list markers:
```
* Red
* Green
* Blue
```
```
+ Red
+ Green
+ Blue
```
```
- Red
- Green
- Blue
```

will get the same result:  
* Red
* Green
* Blue


## Ordered Lists

Similarly, you can make an ordered list by preceding list with a number.
```
1. Item1
2. Item2
3. Item3
```

1. Item1
2. Item2
3. Item3

## Nested Lists

You can create nested list by indenting list items by (one or more) space(s).
```
1. Courses
  * Calculus
  * C++
2. Teacher
  1. Spencer
  2. Tom
```

1. Courses
  * Calculus
  * C++
2. Teacher
  1. Spencer
  2. Tom

# Lesson5 Blockquotes and Paragraphs

## Blockquotes

If you need to call special attention to a quote from another source, or design a pull quote for a magazine article, then Markdown's _blockquotes_ syntax will be useful. A blockquotes is a sentence or paragraph that's been specially formatted to draw attention to the reader. For example:
> Keep it simple, stupid.           --U.S.Navy

To create a blockquotes, all you have to do is preface a line with (>):
```
> Keep it simple, stupid.           --U.S.Navy
```

Blockquotes can be nested by adding additional levels of (>):
```
> This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.
```

> This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.
```

## Paragraphs

### Hard Break

A paragraph is simply one or more consecutive lines of text, separated by one or more blank lines(a line containing nothing but spaces or tabs). Normal paragraphs should not be indented with spaces or tabs.

```
On July 2, an alien mothership entered Earth's orbit and deployed several dozen saucer-shaped "destroyer" spacecraft, each 15 miles (24 km) wide.

On July 3, the Black Knights, a squadron of Marine Corps F/A-18 Hornets, participated in an assault on a destroyer near the city of Los Angeles.
```

becomes:  
On July 2, an alien mothership entered Earth's orbit and deployed several dozen saucer-shaped "destroyer" spacecraft, each 15 miles (24 km) wide.

On July 3, the Black Knights, a squadron of Marine Corps F/A-18 Hornets, participated in an assault on a destroyer near the city of Los Angeles.

### Soft Break

Suppose you want to write text that looks like this:

All that is gold does not glitter;  
all that is long does not last;  
All that is old does not wither;  
not all that is over is past.

You can accomplish this by inserting two (or more) spaces after each new line.
```
All that is gold does not glitter;##
all that is long does not last;##
All that is old does not wither;##
not all that is over is past.
```
Each hash(#) represents a space on the keyboard.

# Lesson6 Code

## Inline Code

To create inline code, warp it with backtick quotes(`). For example:
```
Use the `printf()` function.
```

will produce:  
Use the `printf()` function.

### Code Blocks

GFW also supports fenced blocks. Just wrap your code in ```(as shown below).
    ```
    function test() {
        console.log("notice the blank line before this function?");
    }
    ```

becomes:  
```
function test() {
    console.log("notice the blank line before this function?");
}
```

### Syntax highlighting

Code blocks can be taken a step further by adding syntax highlighting. In your fenced block, add an optional language identifier and we'll run it through syntax highlighting. For example, to syntax highlight Ruby code:
    ```ruby
    require 'redcarpet'
    markdown = Redcarper.new("Hello  World!")
    puts markdown.to_html
    ```

becomes:  
```ruby
require 'redcarpet'
markdown = Redcarper.new("Hello  World!")
puts markdown.to_html
```
