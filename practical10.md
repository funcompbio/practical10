---
layout: page
title: Practical 10
permalink: /practical10/
---

# Objectives

The learning objectives for this practical are:

  * Create HTML documents.
  * Create Markdown documents.
  * Create R Markdown documents.

# Setup and background

To do this practical you need an installation of R and RStudio. You can find
the instructions in the [setup](/setup/) link on how to install R and RStudio
in your system.

# HTML documents

The basic skeleton for an HTML document consists of:

1. A [DOCTYPE](https://www.w3schools.com/tags/ref_html_dtd.asp) element
that tells the web browser this is an HTML document:

    ```
    <!DOCTYPE html>
    ```

2. A [head](https://www.w3schools.com/tags/tag_head.asp) element, which contains
metadata, enclosed in other HTML elements, about the whole document
such as a title that is displayed in the browser tab displaying the HTML document.
Another common metadata to be included here is the one associated with the `<style>` element.

    ```
    <head>
      <title>Page Title</title>
    </head>
    ```

3. A [body](https://www.w3schools.com/tags/tag_body.asp) element with the main content
of the HTML document, which in this case consists of a heading and a paragraph.

    ```
    <body>
      <h1>This is a first-level heading</h1>

      <p>This is a paragraph.</p>
    </body>
    ```

The elements in parts 2 and 3 of the skeleton are enclosed by starting `<html>` and ending
`</html>` elements. The whole skeleton together looks as follows:

```html
<!DOCTYPE html>
<html>
<head>
  <title>Page Title</title>
</head>
<body>
  <h1>This is a first-level heading</h1>

  <p>This is a paragraph.</p>
</body>
</html>
```

Copy and paste the previous code into a text file called `myfirstpage.html`,
using a text editor for instance, and open it with the web browser (`File -> Open File ...`).

The basic HTML elements are:

* A text [headings](https://www.w3schools.com/tags/tag_hn.asp): `<h1>`, `<h2>`, ..., `<h5>`, `<h6>`.

* A [paragraph](https://www.w3schools.com/tags/tag_p.asp): `<p>`.

* An [unordered (bulleted) list](https://www.w3schools.com/tags/tag_ul.asp): `<ul>` and `<li>`.

* An [ordered list](https://www.w3schools.com/tags/tag_ol.asp): `<ol>` and `<li>`.

* A [hyperlink](https://www.w3schools.com/tags/tag_a.asp): `<a>` with the `href` attribute specifying the linked file or URL.

* An [image](https://www.w3schools.com/tags/tag_img.asp): `<img>` with the `src` attribute specifying the path to the image file.

* A [single line break](https://www.w3schools.com/tags/tag_br.asp): `<br>`.

* An [horizontal ruler](https://www.w3schools.com/tags/tag_hr.asp): `<hr>`.

Using some of these elements, edit the `myfirstpage.html` file and modify it to
make a web page about your favorite (or unbeloved) music band. The page should
include two sections, one with the origins of the band and its current members
and another with its discography (shorten it to the most relevant one if its long).
Add a picture of the band and a link to their official web page. Try to keep it
under 30 lines. To display it in the web browser you need to (1) save the file in
your text editor and (2) press the reload button in the tab from web browser
where you loaded the page.

## Styling with CSS

You can alter the _style_ of HTML elements using so-called
[CSS](https://en.wikipedia.org/wiki/CSS) declarations. There are different ways
to include them, one of them is through the `<style>` element in the `<head>`
section of the HTML document. For instance, edit your `myfirstpage.html` file
and add the following CSS declaration within the `<head>` section:

```
<style>
h1 {
  font-family: arial;
}
</style>
```
Now reload the page and you should see how the text associated with the first-level
heading `<h1>` elements has changed its font. Consult the following
[link](https://www.w3schools.com/css/default.asp) and change in the file
`myfirstpage.html` the default black color of the first-level heading `<h1>` element
into another one.

# Markdown

We will learn Markdown as follows. In one tab of your browser open the
[CommonMark reference page](https://commonmark.org/help). In another tab
follow the 10-minute [CommonMark tutorial](https://commonmark.org/help/tutorial).

Once you are finished with the tutorial, create a Markdown version of your previous
file `myfirstpage.html`, i.e., a `myfirstpage.md` file, with all the previous content
but formatted using Markdown only. You can create and process Markdown files from
RStudio with the option `File -> New File -> Markdown File`. To process and visualize
the file click on the `Preview` button of the source code editor.

As an alternative to RStudio as Markdown editor, you can download and install the
Markdown editor and reader [typora](https://typora.io).

# R Markdown

Go to RStudio and create a new R Markdown file by doing `File -> New File -> R Markdown ...`
with the default option for output format (HTML). Give the text `COVID19 Analysis` as title.
You will get a sample R Markdown file, press the `knit` button on top of the source code
panel (see image below with a red arrow pointing to that button).

![](rstudioknitbutton.png)

After processing the file, a popup window should appear displaying the HTML page of
the R Markdown file. Now modify this file to contain the analysis of the COVID19 data
from [practical 9](/practical 9/) or, alternatively, the analysis of the COVID19 data
of the current assignment. The final R Markdown document should contain:

1. Some text explaining each different data processing steps.
2. At least one figure.
3. At least one table with the numerical results.

In the following [link](https://rmarkdown.rstudio.com/lesson-1.html) you can find a
comprehensive description of the R Markdown language. In the section
[Tables](https://rmarkdown.rstudio.com/lesson-7.html) you can find a way to pretty
print the table with numerical results. In this other
[link](https://rmarkdown.rstudio.com/authoring_basics.html) you have a quick reference
to the most commonly used R Markdown syntax. The `Help` menu of RStudio also has links
to many resources including cheatsheets for R Markdown.

# Epilogue

While not strictly required or necessary for FCB, you are now equipped to create your own
public website. Because you are already working with a GitHub account, you can easily
do it with [GitHub Pages](https://pages.github.com). A very well paced guide to use GitHub
Pages is the one by [Jonathan McGlone](http://jmcglone.com/guides/github-pages). Another
even easier option to publish HTML files in a public website is
[Netlify Drop](https://app.netlify.com/drop), which can be handy if you need to quickly
share a website.
