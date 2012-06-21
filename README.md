iBooks-KF8
==========

Python script to convert iBooks fixed layout to KF8 files

==THIS IS A WORK IN PROGRESS==

If anyone has any suggestions for simplifying this code it would be gratefully recieved.
It does work, as long as all the conditions below are met.
If you run into any serious issues let me know.

  * File for conversion must be placed in /files folder
  * Output place in /repubbed folder
  
Usage: Navigate to scripts file in the command line, then type "python ibooks_kf8.py"

Things you need for this to work:

  * Python 3+ and BeautifulSoup4 module installed
  * Folder structure must be as it is on git
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