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

We will download some COVID19 data to illustrate the use of R and RStudio.
Please follow the next two steps:

1. Go to the Catalan Health Departament COVID19 data portal at
   [https://dadescovid.cat](https://dadescovid.cat) and switch the language to
   "ENGLISH" using the pull-down menu on the top-right corner of the page.
2. Follow the downloads link and on the next page click and download the file
   corresponding to the "7 DAY AGGREGATION" for "CATALUNYA".
   Make sure you know exactly where in your filesystem this file
   has been downloaded. **Tip:** some browsers automatically download files
   into a folder called "Downloads" or under a name corresponding to the
   translation of "Downloads" to the default language of your operating system.
3. Make a directory in your filesystem, for instance at your _home_ directory,
   called `practical10` and copy in it the downloaded file.
4. Since the downloaded file is a ZIP file, uncompress as you did in
   [practical 1](/practical1/) so that you finally have a file called
   `catalunya_setmanal.csv` in the directory `practical10`.

If you are using the UPF _myapps_ cloud to run RStudio, then you need to
either use an internet browser in _myapps_ to download the data file directly
in the _myapps_ cloud or upload to the _myapps_ cloud the file that you have
downloaded in your own computer.

# HTML documents

The basic skeleton for an HTML document has the following form:

```html
<!DOCTYPE html>
<html>
<head>

   <!-- head definitions go here -->

</head>
<body>

   <!-- the content goes here -->

</body>
</html>
```
