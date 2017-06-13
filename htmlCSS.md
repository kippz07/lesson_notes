# HTML and CSS

---

**HTML** - HyperText Markup Language

**CSS** - Cascade Style Sheets

***\<!- -*** *comment* ***- ->*** or **(cmd + /)** - make a comment in html

***<!DOCTYPE html>*** - write this on the first line

***\<html>, \</html>*** - start, end of a HTML document

***\<head>*** - where you put information about the html file, like the title

***\<body>*** - where the main content goes

***\<p>*** - paragraphs

***\<div>*** - lets you divide up the page into containers

***\<span>*** - allows you to contraol stying for smaller parts of the page, individual words/sentances in a paragraph for example

***\<h1> - \<h6>*** - headings, h1 is the largest and h6 is the smallest

***\<a href="****link_address****">****Link description****\</a>*** - create a link

***\<img src="****image_source****"/>*** - add image

Images can be made into links by putting the img tag as the link description

--

***\<ol>*** - make an ordered list

***\<ul>*** - make an unordered list

***\<li>*** - create a list item in a list

--

***\<p style ="font-size:12px">*** - add a style, in this case the font size, to an element, here p

**Not recommended to add styles in HTML, instead use CSS**

***\<strong>*** - makes enclosed text bold

***\<em>*** - makes enclosed text italic

--

***\<table>*** - add a table

***\<tr>*** - add a row to a table

***\<td>*** - add a column in a row

***\<thead>*** - contains information about the table

***\<tbody>*** - contains the tabular data

***\<th>*** - for column heading

***colspan="n"*** - make row spread across n columns

---

**CSS can be put in a \<style> tag in the \<head> section or in a sepearte file which is then linked**

**\<link type="text/css" rel="stylesheet" href="ref to css file"/>**

**/\*CSS comment\*/** or **(cmd + /)**

**p {  
color: blue;** - assign a style to an element , \<p> in this case  
**}**

***font-size:*** *12px* - change the font size to 12 px

***color:*** *blue* - changes the font colour to blue

***font-family:*** *Impact* - changes the font

***background-color:*** *red* - changes the background colour

***text-align:*** *center* - aligns the text center

***border:*** *1px dashed black* - adds a border to the element

***text-decoration:*** *none* - 'none' removes the underline from a text link

***border-radius:*** *5px* - sets how rounded you want the border edges

***margin:*** *auto* - centers the element

--

**div div div p { }** - only style the \<p> that are nested inside 3 \<div>'s

**\* {  }** - styles every element on the page

**div > p { }** - only elements of \<p> that are direct children of \<div> are styled

--

**Classes** - for when you have a bunch of elements that should all recieve the same styling

**IDs** - for when you have exactly one elmemnt that should recieve a certain kind of styling

***\<p class="class_name">*** - assigning a class in HTML

**.class_name {  }** - class identified with a "dot" in CSS

***\<p id="id_name">*** - assigning an ID in HTML

**#id_name { }** - ID identified with a hash in CSS

--

**Pseudo-class selector** - a way of accessing html items that arent part of the document tree

**a:hover { }** - apply styles when \<a> is hovered over

**a:link { }** - apply styles to an unvisited link

**a:visited { }** - apply styles to a visited link

**p:first-child { }** - apply styles to only the first child of the parent

**p:nth-child(x) { }** - apply styles to the nth child, replace x with the child number

--

**display:block** - element takes up the full width of page and is formatted as a block

**display:inline-block** - allows ther elements to sit next to it on the same line

**display:inline** - element sits on the same line as another element but is not formatted as a block

**display:none** - element and content disappears form the page entirely

**float:***right/left* - tells the element where to go on the page

**clear***right/left/both* - element moves below floating elements on the selected side of the page/ both sides of page

**position:absolute** - element is positioned to the first parent element that is not static

**poition:relative** - tells ement to move relative to where it whould have landed in static

**position:fixed** - anchors the element to the page, stays there even when scrolling

**z-index:1** - the lower the z-index, the higher it will be stacked on the page. z-index:1 will be on the top