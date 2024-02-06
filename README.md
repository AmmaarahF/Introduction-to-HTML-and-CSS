# Introduction-to-HTML
==================================================================

What is html ? 
Html, known as Hypertext Markup Language, is a markup language crucial for building and designing web pages. It structures content using tags, defining elements and their relationships like headings, paragraphs, and links, enabling browsers to render information.

What is css ?
CSS, known as Cascading Style Sheet, is a coding language essential for web development. It dictates the visual aspects of a website, determining how elements like test, images, layouts appear, ensuring a consistent and attractive user interface.

What is JavaScript ?
JavaScript is versatile but mainly used for web development. It enables dynamic content, interactivity, and asynchronous behavior on browsers. As a client-side scripting language, it manipulates the Document Object Model (DOM) to create responsive and engaging user interfaces.

What is Document Object Model (DOM) ?
DOM is a web development concept where a document’s structure is represented as tree of objects. JavaScript interacts with DOM, enabling dynamic manipulation of webpage content. 

HTML TEXT FORMATING
====================================================================

- Inline elements are elements are meant to wrap around phrases of text that are inline with other content.

Basic elements in HTML (all elements are wrapped in entities)
-------------------------------------------------------------
- h1 - first headline
- h2 - second headline
- p - for paragraphs
- em - for text to appear Italic (used to grab attention ) 
- I - for text to appear Italic (used for visuals like titles) 
- strong - for text to appear bold (to show importance and urgency)
- b - for text to appear bold (used for generic and neutral purposes)


Headlines
-------------------------------
- There are six different types : h1, h2, h3, h4, h5, h6
- The h1 element is the largest and most prominent, while h6 is the smallest and least attention-grabbing.

HTML Lists (all elements should be closed using their closing tags)
--------------------------------------------------------------------
- there are three types of lists > unordered lists, ordered lists and definition lists
- li - represents a list item (these tags are nested in list tags)
- ul - unordered lists are commonly used (lists items in bullet form) 
- ol - ordered lists are simiar to unordered lists, an ordered list follows a specific order and are numbered.
- dt - stands for definition term 
- dd - stands for definition description
 > both  definition tags must be nested in "dl" tags, which represents the definition lists

HTML Quotes (all elements should be closed using their closing tags)
------------------------------
- blockquote - used to distinguish what is nested inside the tags. Any other tags can be added in the blockquotes tags. 
- cite - renders in italic. This tag defines creative work such as poems or books.
- q - used to automatically add the appropriate quotes to the text.

Date and Time Elements
------------------------------
- date element is written as < time datetime="2025-05-08">May 8, 2025< /time>
- time element is written as < time datetime="14:15:28.5">14:15:28.5< /time>

HTML Code, pre and br (all elements should be closed using their closing tags)
------------------------------------------------------------------------------
- &It ; = <                              
- &gt ; = >
> these are known as entities

- code – changes code to monospace font
- br - adding these tags at the end of a line creates a line break
- pre – wrapping the code in pre elements and placing character’s anywhere will make the character’s stay exactly where it is.
- pre and code can be used together

HTML Superscripts, Subscripts and Small Text (all elements should be closed using their closing tags)
-----------------------------------------------------------------------------------------------------
- sub = placing characters at the bottom
- sup = placing characters at the top
- small = adjusting the size of the code (commonly used for footers)

 HTML Capabilities
================================================

Troubleshooting and Debugging HTML Code
------------------------------------------------
In browsers, there is a way for users to see what is going on with a website's code and performance. To access the developer tools, we can either right-click on the demo and select "inspect element" or opt to go to "tools," then "web developer," and choose "inspector." This will open up the developer tools, which offer a wide range of tabs with different tools or controls as it is sometimes also referred to.

-if there's an error in your code, the page will render around the error, trying to fix it.

HTML Attributes (these tags uses closing paragraph tags)
----------------------------------------------------------
- class attribute < p class="intro" >
 > The class attribute is the most commonly used. It allows us to assign a reusable name to any element, which can then be styled using CSS for all elements sharing that class.
  
- id attribute < p class="intro"
                 id="article-intro">
> Can only use unique names once on an entire HTML page. IDs can be used for CSS targeting, but are more specific, which can sometimes cause issues.
> The "dir" attribute explicitly indicates the direction in which the text flows, using "LTR" for left-to-right scripts and "RTL" for right-to-left scripts.


ARIA Roles
-------------------------------------------------------
- ARIA Roles are extra attributes that we can add to HTML elements to make them more meaningful and help browsers understand what they represent.
- ARIA Roles come into play when we want to provide essential information to assistive technologies like screen readers, braille displays, and magnifiers to ensure a website is fully accessible.
  

Formatting HTML
-------------------------------------------------------
- use style tages and css to modify whitespace
- use "<!--" at the start and "-->" at the end to comment in the actual code, the website does not render comments.


Unusual Characters
--------------------------------------------------------
- Character entity are formatted as an ampersand, a short code, and a semicolon. When we include these in HTML, they are transformed into specific characters.
- Example - &copy ; (no spaces) becomes &copy;
- We can use the code "&nbsp;" to insert a non-breaking space between the two names, ensuring they stay on the same line.


HTML Links
-------------------------------------------------------
- When we want to create a link, we use the A element, which stands for anchor.
- To create a link, we need to add ah hred attribute with URL enclosed in quotes.
- href - Hypertext reference
- the A element is inline and can be placed within a paragraph or any other text.
- Absolute URL - a complete web address that spcifies the exact location of a file on the internet, including protocol, domain name, and the path to the specific file.
-  The "S" in HTTPS stands for Secure.
-  In an absolute URL, the HTTP or HTTPS part must be included which stands for Hypertext Transport Protocol. This protocol defines the rules for communication on the web and is crucial for linking.


HTML URL Pathways 
-----------------------------------------------------
- relative URL - a URL that indicates a file's location based on it's relationship to the current directory, streamlining navigation within a project
- absolute URL - a complete web address that specifies that exact location of a file on the internet, including the protocol, domain name, and the path to the specific file.

Creating Local URLs (relative URLs)
-----------------------------------------------------
1. /images/logo.gif
2. ../images.logo.gif

   1 - relative to the root level. The browser will start looking for the specific file from the root of the website.<br>
   2 - relative to the location of the file where URL is written. The ".."means going up one level in the directory structure


Navigation
----------------------------------------------------
- when making a menu navigation, each link is wrapped in an element with the correct URL and enclosed in an "li" element to create a list.
- the entire menu should be enclosed with a "nav" element to indicate that it is the navigation.
- to create a footer with links, all links should be enclosed with a "footer" element


HTML Working with Graphics and Images
----------------------------------------------------
Images
------------
- There are four attributes to include when adding an image
  ---------------------------------------------------------
  -  the source attribute (SRC), tells the browser which image to load
  -  alt attribute (ALT) - provides a text description
  -  width and height attributes - determines the size of the image

Image Formats
----------------------------------------------------
- GIF
  > for compressing illustrations that have large areas of same color
- SVG
  > perfect for logos, icons, and other types of illustrations. 
- JPG
  >  for compressing photographs.
- PNG
  >  works well when you need transparency in a photograph, displays in large size without pixelation.

  
Responsive Images 
---------------------------------------------------
- The browser and operating system, takes into account the devices's hardware capabilities and network speed to decide which image to download.
- Even if someone has a high-resolution screen, the browser might opt to download a lower-resolution image.
- To provide the browser with choices, simply add a source set attribute. Inside it, list the images on offer, separated by commas.


Responsive Width
---------------------------------------------------
- indicate width 480w (480 pixels wide) and 960w
- the browser decides which image to show based on device density and viewport width.


Responsive Pictures
---------------------------------------------------
- if you want an image to appear differet sizes on different devices, you should list alternative options using the source element within the picture element.
- for example , if you want two options, there should be two source elements.
- the first source element , use the source set attribute to point to a mobile image file. This will use the cropped version of the photo, sized at 320 pixels.
- the second source element, uses media query for larger screens. If the viewpoint is atleast 600 pixels wide, the landscape version of the photo will load.


Figcaption and Figures
-------------------------------------------------
- Use the figcaption element to wrap the text and designate it as a caption. Then, put the image and the caption together in a figure element.
- Figures can be used for more than just images, too. For example, use them for an interactive graphic. Place it in the same spot where the image element is in the code.


Working With Media
------------------------------------------------
Audio
---------------------------------------
- has opening and close tags
- different audio file formats
  - mp3
- you can create your own using JavaScript and the HTML media element API. For now, add "controls" attribute.
- If the attribute is present, it means we want the controls.

Video
--------------------------------------
- has opening and close tags
- To display a video, use the source attribute to specify the video file.
- Various codecs developed
  > Real Video
  > Sorenson
  > Windows Media
  > Flash
  > H.263
  > H.264 - patented codec owned by a consortium


Working With Captions and Subtitles
------------------------------------------------
- adding the track element and linking it to a text file to add captions to the video.
- this element adds functionality to the video player, allowing users to toggle captions on and off or switch between different subtitle options.
- On the web, a file format called ibvtt, which stands for web video text tracks, will be used. It is a simple text file with a vtt extension that follows a specific convention for providing information.
- To display these captions on the video, insert a track element within the video element.
- On the track element, use the source attribute to specify the file.
- Use the source lang attribute to indicate the language and add a default attribute to make this track the default choice when captions are enabled.


Embedding Media via Iframes
--------------------------------------------------
- iframe element has attributes like height and width that can be adjusted.
- The src attribute is used to specify the source of the video file.
- embedded someone else's toolkit onto your own website

HTML Content Identification
--------------------------------------------------
HTML Language Support 
-------------------------------
- The lang attribute is used to specify the language of a webpage.
- The lang attribute also indicates the writing system used.
- do not forget to set the charset (set of characters)
- To specify the charset in HTML, simply include a meta charset tag that equals UTF-8. Place this meta element within the head element on every page of the website.


HTML Generic Elements, Div and Span
--------------------------------------------------
- avoid using divs and spans for every little thing.
- Div is a block-level element, while span is an inline element , They do nothing until CSS or Javascript is applied to them.
- Both div and span can make use of various global attributes like class, id, lang, and aria roles.


HTML Integration
-------------------------------------------------
HTML Page
---------------------
- CSS is in css files
- JavaScript is in JavaScript files
- Additional files for images, video, audio, an ads.
<br>
- Users visit a URL > prompts a request for an HTML file > server returns a single HTML file > browser reads a HTML file and follows it's instructions. <br>
- that initial HTML file that is returned when a web page is requested serves as a central hub for everything that happens after the site first loads.

<strong> Once the HTML file is built, there are a few crucial parts that every web page needs. </strong><br>
- the file should begin with a doctype statement (indicates era)
- enclose everything else on the page within an HTML element (< HTML >)
<br>
- declare language being used and the content flow direction
- Inside the HTML element, there are two main parts where everything goes: the head and the body.
  >  The head contains all the metadata that the browser needs to know but will not display on the page.
  >  The body is for all the content and is composed of various elements
  > The doctype declaration, HTML head, and body elements are the essential building blocks of every web page.

Document Head
--------------------------------------------------
- Meta elements are only placed inside the head (they provide metadata about the page)
- to define the character set, use the character set attribute and set it to UTF-8.
- title element > appears on the browser tab or bookmark
- One of the purposes of the meta element is to inform the browser that the layout is responsive.
- Moreover, the meta tag is employed to assign a name to the webpage when saved to the home screen, and to specify a tile image and background color.
- When a link is shared on platforms like, Twitter, it turns into an attractive card.
- the <b>link element</b> serves to connect various assets that should load files such as CSS, fonts, and favicon > To inform the browser about the type of asset, utilize the rel attribute.
- the href attribute is employed to specify the URL for the asset.
- The script tag is used element in an HTML document's head > It instructs the browser to load a JavaScript file.

Content Structuring
---------------------------------------------------
1. Main
 > is used once per webpage and tells the browser where the main content is located.
2. Header
 > Header is used for site headers, article headers, and headers within the content.
3. Footer
 > signifies that there are extra things to convey, regardless of its position on the page.
4. Article
 > An article starts with a title, subtitle, author's name, and publication date, which can also be considered a <b>header.</b>
 > The article element wraps around any type of content unit, whether it is a long written article, a short snippet, a teaser card, a tweet, or even an app element.
 > It represents a standalone unit of content.
5. Section
 > The section element is used to mark sections of content.
 > each segment can be wrapped in a section element
 >  it's useful for dividing different topic zones on a website.
6.


