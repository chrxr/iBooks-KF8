iBooks-KF8
==========

Python script to convert iBooks fixed layout to KF8 files

Things you need for this to work:

  * Python 3+ and BeautifulSoup4 module installed
  * Folder for content must be OPS. I'm working to get this more flexible.
  * Content files must be .xhtml
  * Viewport dimensions in content files must be listed as width then height, without px suffix
  * Cover page should be called cover.xhtml
  * Must include a reset css file called reset.css
  * Best to use RGB Jpg files. Transparent PNG files won't work at all.
  
Things it doesn't do:
  
  * Resolve internal or TOC links: If you have a full NCX TOC the links will have to be changed by hand. The same for HTML TOCs and other internal links
  * Guarantee that things will work: Especially when it comes to SVG. Very likely you'll have to re-do or at least tweak SVG text.
  * Resize anything: Everything will be the same size as it was in iBooks. 