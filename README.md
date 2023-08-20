# kids_bookmaker
A bookdown-based toolkit for kids to make books in html format

## Key files:

* `index.rmd`
  * This file contains the title, author name, and cover page
* `story.rmd`
  * This file is where the story goes
* `about_author.rmd`
  * This file contains the author's biography and other information
* `_output.yml`
  * This file contains the specifications for the table of contents and left information bar
* `style.css`
  * This file contains the HTML formatting rules
* `bookdown.yml`

## Directories:

* `Images/`
  * Add images to this folder. They can then be referenced inline in `index.rmd`, `story.rmd`, `about_author.rmd`, and `_output.yml`.
* `_book/`
  * HTML output files appear here.
  
## Basic changes to make:

* In `index.Rmd`:
  * Title: line 2
  * Author name: line 3
  * Cover picture for story: line 19 (`... img src="images/<FILE NAME>"`)
* In `_output.yml`:
  * Author photograph: line 7
  * Author name: line 8
* In `about_author.rmd`:
  * Author photograph: line 3
  * Author biography: line 6 and subseuqent lines
* In `style.css`:
  * Comment out all color schemes except for the one that you want. Or, if you feel ambitious, make your own.
  * Default color scheme is pastels.
  * Color schemes specify header and sidebar colors
* In `story.rmd`:
  * Write your story
    * To start a new page, start a line with a "#", followed by a chapter name.
    * To start a new section within a page, start a line with "##", followed by a subchapter name.
    * To add a picture, add the following line:
      * `<center><img src="images/<PICTURE_NAME>.png" alt="Author" class="cover" width="500" height="500"/></center>`
      * Replace `<PICTURE_NAME>.png` with the file name and extension of your picture.
      * If you would like your picture to have a caption, start the line above with "###", followed by the picture caption.
