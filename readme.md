# Hello Coder... !! | Markdown for begginer

## **Markdown**

>markdown is a **lightweight markup language** for creating **formatted text** using a **a plain-text editor. john Gruber** abd **Aaron swartz** created Markdown in 2004 as a **markup lanuage** that is appealing to human readers in its source code form. Markdown is widely used in **blogging, instant messaging, online forums, collaborative software, documentation** pages, and **readme files.**

>The initial description of Markdown contained ambiguities and raised unanswered questions, causing implementations to both intentionally and accidentally diverge from the original version. This was addressed in 2014, when long-standing Markdown contributors released **CommonMark,** an unambiguous specification and test suite for Markdown.
        
***

## **Content**

**[1. History](#heading--1)**

**[2. Rise and divergence](#heading--2)**

**[3.Standardization](#heading--3)**

**[4.Variants](#heading--4)**

 - [4.1	GitHub Flavored Markdown](#heading--4-1)

 - [4.2	Markdown Extra](#heading--4-2) 

 - [4.3	LiaScript](#heading--4-3)

 - [5.Examples](#heading--5)



**[6. Implementations](#heading--6)**

**[7. See also](#heading--7)**

**[8. Explanatory notes](#heading--8)**

**[9. References](#heading--9)**

**[10. External links](#heading--10)**

***

## History

***

Markdown was inspired by pre-existing **conventions** for marking up **plain text** in **email** and **usenet posts,** such as the earlier markup languages **setext** 

In 2002 Aaron Swartz created **atx** and referred to it as “the true structured text format”. Swartz and Gruber then worked together to create the Markdown language in 2004, with the goal of enabling people "to write using an easy-to-read and easy-to-write plain text format, optionally convert it to structurally valid **XHTML** (or **HTML**)

Its key design goal was readability, that the language be readable as-is, without looking like it has been marked up with tags or formatting instructions, unlike text formatted with ‘heavier’ markup languages, such as **Rich Text Format**(RTF), **HTML,** or even  **wikitext** (each of which have obvious in-line tags and formatting instructions which can make the text more difficult for humans to read).

Gruber wrote a **Perl** script, Markdown.pl, which converts marked-up text input to valid, **well-formed**XHTML or HTML and replaces angle brackets (<, >) and **ampersands** (&) with their corresponding **character entity references.** It can take the role of a standalone script, a plugin for **Blosxom** or a **Movable Type,** or of a text filter for **BBEdit.**

***

## Rise and divergence

***
As Markdown's popularity grew rapidly, many Markdown implementations appeared, driven mostly by the need for additional features such as tables, footnotes, definition lists, and Markdown inside HTML blocks.

The behavior of some of these diverged from the reference implementation, as Markdown was only characterised by an informal specification and a Perl implementation for conversion to HTML.

***
## Standardization

***

![Markdown](/markdown%20logo%20png.jpg) 

```
Filename extensions:  .md, .markdown 

Internet mediatype:	text/markdown; variant=CommonMark

Developed by :	 John MacFarlane, open source

Initial release: October 25, 2014 (7 years ago)

Latest release : June 19, 2021 (14 months ago) 

Type of format :	Open file format

Extended from :	Markdown

Extended to	: GitHub Flavored Markdown
```

- ## [Website](spec.commonmark.org)





From 2012, a group of people, including **Jeff Atwood** and **John MacFarlane,**  launched what Atwood characterised as a standardisation effort. A community website now aims to "document various tools and resources available to document authors and developers, as well as implementors of the various Markdown implementations".In September 2014, Gruber objected to the usage of "Markdown" in the name of this effort and it was rebranded as CommonMark. CommonMark.org published several versions of a specification, reference implementation, test suite, and "**plans** to announce a finalized 1.0 spec and test suite in 2019."No 1.0 spec has since been released as major issues still remain unsolved.

***
## Variants
***

Websites like **GitHub,Bitbucket, Reddit,Diaspora, Stack Exchange, OpenStreetMap** and **SourceForge**  use variants of Markdown to facilitate discussion between users. Markdown is also supported in a wide variety of apps and services, like **Microsoft Teams**  chat and **Discord** messages.

Depending on implementation, basic inline **HTML tags**  may be supported.Italic text may be implemented by ```_underscores_ ```and/or  ```*single-asterisks*.```

**GitHub Flavored Markdown**
```
GitHub had been using its own variant of Markdown since as early as 2009,adding support for additional formatting such as tables and nesting block content inside list elements, as well as GitHub-specific features such as auto-linking references to commits, issues, usernames, etc. In 2017, GitHub released a formal specification of its GitHub Flavored Markdown (GFM) that is based on CommonMark. It is a strict superset of CommonMark, following its specification exactly except for tables, strikethrough, autolinks and task lists, which GFM adds as extensions. GitHub also changed the parser used on their sites accordingly, which required that some documents be changed. For instance, GFM now requires that the hash symbol that creates a heading be separated from the heading text by a space character.
```

**Markdown Extra**
```
Markdown Extra is a lightweight markup language based on Markdown implemented in PHP (originally), Python and Ruby.It adds features not available with plain Markdown syntax. Markdown Extra is supported in some content management systems such as, for example, Drupal and TYPO3.
```

**Markdown Extra adds the following features to Markdown**:

 - [Markdown markup inside HTML blocks](#heading--1)

 - [Elements with id/class attribute](#heading--2)

 - ["Fenced code blocks" that span multiple lines of code](#heading--3)


 - [Tables](#heading--4)

 - [Definition lists](#heading--5)

 - [Footnotes](#heading--6)

 - [Abbreviations](#heading--7)

## LiaScript
```
LiaScript[43] is a Markdown dialect that was designed to create interactive educational content. It is implemented in Elm and Typescript and adds additional syntax elements to define features like:

 Animations

 Automatic speech output

 Mathematical formulas (using KaTeX)

 ASCII art diagrams

 Various types of quizzes and surveys

JavaScript is natively supported and can be   attached to various elements, this way code  fragments can be made executable and editable
```

***
## Examples
***

**Text using Markdown syntax**
```
Heading
=======

Sub-heading
-----------

# Alternative heading #

Paragraphs are separated 
by a blank line.

Two spaces at the end of a line  
produce a line break.
```
```
Text attributes _italic_, **bold**, `monospace`.

Horizontal rule:

```

```
Bullet lists nested within numbered list:

  1. fruits
     * apple
     * banana
  2. vegetables
     - carrot
     - broccoli
```

```
A [link](http://example.com).

![Image](Icon-pictures.png "icon")

> Markdown uses email-style
characters for blockquoting.
>
> Multiple paragraphs need to be prepended individually.

Most inline <abbr title="Hypertext Markup Language">HTML</abbr> tags are supported.
```

## Corresponding HTML produced by a Markdown processor

```
<h1>Heading</h1>

<h2>Sub-heading</h2>

<h1>Alternative heading</h1>

<p>Paragraphs are separated
by a blank line.</p>

<p>Two spaces at the end of a line<br />
produce a line break.</p>
```

```
<p>Text attributes <em>italic</em>, <strong>bold</strong>, <code>monospace</code>.</p>

<p>Horizontal rule:</p>

<hr />
```

```
<p>Bullet lists nested within numbered list:</p>

<ol>
  <li>fruits <ul>
      <li>apple</li>
      <li>banana</li>
  </ul></li>
  <li>vegetables <ul>
      <li>carrot</li>
      <li>broccoli</li>
  </ul></li>
</ol>
```

```
<p>A <a href="http://example.com">link</a>.</p>

<p><img alt="Image" title="icon" src="Icon-pictures.png" /></p>

<blockquote>
<p>Markdown uses email-style characters for blockquoting.</p>
<p>Multiple paragraphs need to be prepended individually.</p>
</blockquote>

<p>Most inline <abbr title="Hypertext Markup Language">HTML</abbr> tags are supported.</p>
```

## Text viewed in a browser

```
Heading

Sub-heading

Alternative heading

Paragraphs are separated by a blank line.

Two spaces at the end of a line
produce a line break.
```

```
Text attributes italic, bold, monospace.
Horizontal rule:
```

```
Bullet lists nested within numbered list:
1. fruits
  apple
  banana
2. vegetables
  carrot
  broccoli
```

```
 link.
Image

Markdown uses email-style characters for blockquoting.

Multiple paragraphs need to be prepended individually.

Most inline HTML tags are supported.
```
***
## Implementations
***

Implementations of Markdown are available for over a dozen programming languages; in addition, many platforms and frameworks support Markdown.For example, Markdown plugins exist for every major blogging platform.

While Markdown is a minimal markup language and is read and edited with a normal text editor, there are specially designed editors that preview the files with styles, which are available for all major platforms. Many general purpose text and code editors have syntax highlighting plugins for Markdown built into them or available as optional download. Editors may feature a side-by-side preview window or render the code directly in a **WYSIWYG** fashion.

 - **JotterPad** : an online WYSIWYG editor that supports Markdown and fountain

 - **Doxygen** : a source code documentation generator which supports Markdown with extra features.

 - **RStudio** : an IDE for R. It provides a C++ wrapper function for a markdown variant called sundown

 - **GitHub Flavored Markdown (GFM)**  ignores underscores in words, and adds syntax highlighting, task lists, and tables.

 - **RMarkdown**

 - **Nextcloud Notes** : the default app for taking notes on the Nextcloud platform supports formatting using Markdown

 - **Joplin** : a note-taking application that supports markdown formatting

 - **Simplenote**

 - **Obsidian.md**

 ***
 ## See also
***

   - **[Comparison of document markup languages](#heading--1)**

  - **[Comparison of documentation generators](#heading--2)**

  - **[Lightweight markup language](#heading--3)**

  - **[Wiki markup](#heading--4)**

***
## Explanatory notes
***
  
Technically HTML description lists.


## References
***

 - ****"Un naufragio personal**: The Grutatxt markup". triptico.com. Retrieved 2022-06-30.

  - **"EtText: Documentation**: Using EtText". ettext.taint.org. Retrieved 2022-06-30.

  - **"Markdown Syntax Documentation"**. Daring Fireball.

  - **"GitHub Flavored Markdown Spec** – Why is a spec needed?". github.github.com.

  - **"Babelmark 2** – Compare markdown implementations". Johnmacfarlane.net. Retrieved 2014-04-25.

  - **"Babelmark 3** – Compare Markdown Implementations". github.io. Retrieved 2017-12-10.

  - **"Babelmark 2** – **FAQ"**. Johnmacfarlane.net. Retrieved 2014-04-25.

***
## External links
***

  - [Official website](#heading--1)  for original John Gruber markup.


    
    
## **Thanks for Readings..**

