
Requirements
* Single base file format
	* From which all other formats are derived
		 * Necessary for handling bug fixes
	* Human readable so it can serve as the base "raw text" format
	* Markup for the main bdy text should be minimal
		* Not HTML
* Generate other formats automatically from base format
	* -> html, ebook, kindle, ...
* Self contained (other than images, if any)
* Proper support for large and small displays (desktop and mobile)
* Clean images:
	* transparent background (for flexibility with background color)
	* medium to high resolution
	* scale appropriately for display size
* Clean presentation:
	* off-white and off-black to reduce harsh contrast
* Modern UX
	* footnote handling as sidenotes or inline
	* easy to find chapter and paragraph links for cross-referencing
* accessibility
	* aria tags
	* skip to main content
	* how to handle footnotes
	* See https://css-tricks.com/the-checkbox-hack/
	* See https://ffoodd.github.io/a11y.css/
	* See https://www.smashingmagazine.com/2013/08/semantic-css-with-intelligent-selectors/
	* See https://developer.paciellogroup.com/blog/2016/01/the-state-of-hidden-content-support-in-2016/

Gutenberg
* No consistency with generated formats (eg, html)
* (Apparently) no base raw format from which all others are derived

* LA CITÉ DE CARCASSONNE
* http://www.gutenberg.org/files/18940/18940-h/18940-h.htm
	* Images are scaled according to display width, not the font size.
	* Images are low quality
	* Text width and margins are based on the size of the display (with no minimum
		or maximum enforced), so lines are too long to read comfortably
		when the display is wide and margins are too wide when the display is narrow.
	* Footnotes converted to endnotes.
* Dictionnaire raisonné de l'architecture française du XIe au XVIe siècle (1/9)
* http://www.gutenberg.org/files/30781/30781-h/30781-h.htm
	* Hard-coded width. Text and images are cut off on narrow displays (like mobile)
	* Images: low quality; non-transparent background; hard-coded size

* Convenient Houses, by Louis Henry Gibson
* http://www.gutenberg.org/files/42469/42469-h/42469-h.htm
* Release Date: April 5, 2013 [eBook #42469]
	* Text width is percentage of display, so it is too wide on large displays.
	* Images; hard-coded image size; non-transparent
	* Page anchors, but no easy way to get page link.
	* Inline footnotes
	* Character set encoding: ISO-8859-1
	
* LIFE IN THE MEDIEVAL UNIVERSITY
* http://www.gutenberg.org/files/20958/20958-h/20958-h.htm
* Release Date: April 2, 2007 [EBook #20958]
	* footnote -> endnote
	* Character set encoding: ISO-8859-1
	* hard-coded image size
	* text width is percentage of display (so too wide)
	* HTML links are absolute, so local copies link to the gutenberg.org file (browser fault?)
	
* Kellogg's Great Crops of Strawberries
* http://www.gutenberg.org/files/57123/57123-h/57123-h.htm
* Release Date: May 9, 2018 [EBook #57123]
	* hard coded image sizes
	* text width percentage
	* page markers, but no links
	* Page names spelled out. why? e.g., "Page twenty-six"
	* Good: relative links (check)


Archive.org
* Raw image files and auto OCR text documents.
* But
	* Multiple copies of many books which is good for comparison


Readable rich-text formats

Markdown, ASCIIdoc
	* poor handling of Footnotes


Inline notes:
	* https://medium.com/@bnjmnbnjmn/in-line-notes-with-only-html-css-f181c5ceef59
	* https://github.com/edwardtufte/tufte-css