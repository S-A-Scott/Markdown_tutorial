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

# Markdown Basics


## What is Markdown

[Markdown](daringfireball.net/project/markdown) is a way to style text on the web. You control the display of the document; formatting
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
For example, input
```
**_This text will be italics and bold_**
```

will output:__
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

will output:__
# Header one
## Header two
### Header three
#### Header four
##### Header five
###### Header six

# Lesson2 Links
