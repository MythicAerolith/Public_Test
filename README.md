# Public_Test
Test for practicing repositories and collaboration 

LANGUAGE NOTES



HTML (Hypertext Markup Language): determines how a webpage looks and is formatted, content  & layout, create the basic structure of website

CSS: satatic programming language, styling and look, popular sheet style language (colors, fonts, layout, responsive fts), make more visually appealing

JavaScript: Interactive Elements, allows you to change both CSS and HTML elements on web after site has been loaded, ability to add animations,
embedded video media

to focus on improving FRONT-END elements of website, the most important languages to learn include, HTML5, CSS3, Bootstrap, and Javascript
for BACK-END, use Python, Ruby, and PHP

HyperText- text displayed on computer or device that provides access to other text through hjyperlinks
Markup Language- a computer language that defines the  structure and presentation of raw text


                                                                HTML
HTML is a declarative language, meaning it describes a desired result without explicitly listing steps that must be performed. Declarative languages tell an interpreter what to do, not how to do it.


It is best to start thinking about how your website will be structured by considering the heading hierarchy, which would be defined by the h1-h5 tags to create structure visually and verbally for screen readers. You want to avoid skipping headings in order to keep the accessibility level high, skipping headings can create a confusing navigational experience for those using assistance like screen readers. 

Semantic HTML uses tags which best convey the underlying meaning of the content the tag contains.

Browsers style our headings automatically because they have their own CSS built-in.

You want to keep the structure of your HTML coherent for readability, accessibility, and ease of styling.

Dvitis: the excessive misuse of divs to markup a page

Indentation: most style guides recommend that you use two spaces to indent nested elements.


HTML is organized as a collection of family tree relationships. When an element is contained inside another element, it is considered the "child" of that element. The child element is said to be "nested" inside of the "parent" element. 
Example:

<body>
  <h1>Hello World</h1>
  <p>This paragraph is a child of the body element</p>
  <div>
    
  </div> 
</body>

the <body> element is the parent element of the <div> element, and both the <h1> and <p> elements are the child elements nested in the <div> element. <h1> and <p> are at the same level, so they are considered siblings and are both grandchildren of the <body> 


<div> element (short for division) container that divides the page into sections


<section> element is also a container, but it has more meaning semantically unlike the <div> element


Attributes: content added to the opening tag of an element to provide info, change styling, etc. 
"id" is the most common attribute added to elements.
Example:
<div id="intro">
    <h1>Introduction</h1>
</div>
This way, it helps identify the elements when using the same element multiple times


Paragraphs <p>: contains a block of plain text
<span>: contains short pieces of text or other HTML, used to spearate small pieces of content that are on the same line as other content
Example:
<div>
  <h1>Technology</h1>
</div>
<div>
  <p><span>Self-driving cars</span> are anticipated to replace up to 2 million jobs over the next two decades.</p>
</div>



You can use the unordered list tag <ul> to create a list of items in no particular order. An unordered list outlines individual list items with a bullet point. The <ul> element should not hold raw text and won't automatically format raw text into an unordered list of items. Individual list items must have the <li> tag. 
Example:
<ul>
  <li>Limes</li>
  <li>Tortillas</li>
  <li>Chicken</li>
</ul>


Ordered lists <ol> are like unordered lists except each list item is numbered, useful for listing steps or ranking items. You can use the same <li> tag to list individual items.
Example:
<ol>
  <li>Preheat the oven to 350 degrees.</li>
  <li>Mix whole wheat flour, baking soda, and salt.</li>
  <li>Cream the butter, sugar in separate bowl.</li>
  <li>Add eggs and vanilla extract to bowl.</li>
</ol>


You can also style text using HTML tags like <em> to emphasize text, and <strong> to hightlight important text. Browsers have built-in style sheets that will generally style <em> as italic text and <strong> as bold text. 
Example:
<p><strong>The Nile River</strong> is the <em>longest</em> river in the world, measuring over 6,850 kilometers long (approximately 4,260 miles).</p>


To alter spacing, one element used is the <br> or line break element, it use unique because it is only composed of a starting tag. 
Example:
<p>The Nile River is the longest river <br> in the world, measuring over 6,850 <br> kilometers long (approximately 4,260 <br> miles).</p>


In order to add images to your website, you can use the <img> element. This element is self-closing. 
Example:
<img src="image-location.jpg" /> OR <img src="image-location,jpg">

Self-closing tags may include or omit the final slash - both will render correctly.
The <img> tag has a required attribute called "src", which must be set to the source of the image AKA file location, in this case it is the URL (uniform resource locator). A URL is the web address or local address where a file is stored.


The "alt" attribute, which means alternative text, can be added to the image tag just like the "src" attribute to give a text description of the image. It is usually used with assistive technology interactions in mind like when a screen reader comes across an image. The "alt" attribute can also play a role in SEO (search engine optimization) as search engines don't "see" images but read the text. Having descriptive "alt" attributes can improve site ranking.
Example:
<img src="#" alt="A field of yellow sunflowers" />


In order to display videos using HTML, use the <video> element. It also requries the "src" attribute, but it DOES require an opening and closing tag unlike the <img> element. After the "src" attribute, the "width" and "height" attributes set teh size of the video displayed. The "controls" attribute adds basic video controls such as pausing and playing. 
The text, "Video not supported" will only be displayed if the browser is unable to load the video.
Example:
<video src="myVideo.mp4" width="320" height="240" controls>
  Video not supported
</video>


HTML files rewquire certain elements to set up the document properly, we let web browsers know that we are using HTML by starting our doucment with a "document type declaration"
Example:
<!DOCTYPE html>
this decalaration is an instruction, and it must be the first line of code in your HTML document. 
HTML code is always saved in a file with an .html extension.


The <!DOCTYPE html> declaration provides the browser with two pieces of info (type of document and the HTML version), but in order to create HTML structure and content, we must add opneing and closing <html> tags after declaring <!DOCTYPE html>
Example:
<!DOCTYPE html>
<html>

</html>


the <head> elemenet contains the metadata for a web page, metadata is info about the page that isn't displaeyd directly, and it part of the metaphor for the body like <head> = head of person, the brain, thoughts and logic you can't see happening whereas <body> = body of person, the part you can always see.


A browser's ta;b displays the title specified in the <title> tag, and the <title> tag is always inside of the <head>


You can add links to a web page by adding an anchor element <a> and including the text of the link between the opening and closing tags. The anchor must contain the "href" attribute that contains the URL
Example:
<a href="https://www.youtube.com/">YouTube</a>


You can make the link open the webpage in a new tab by using the "target" attribute in the <a> element.
The "target" attribute specifies how a link should open, and to get it to open to a new window it requires a value of "_blank" and the "target" attribute can be added directly to the <a> tag just like the "href" attribute
Example:
<a href="https://en.wikipedia.org/wiki/Brown_bear" target="_blank">The Brown Bear</a>


When making multi-page static websites, web devs often store HTML files in the root directory, or a main folder where all the files for the project are stored. As the size of ypur projects grow, you may use additional folders wihtin the main project folder to organize code. 
Example:
project-folder/
|—— about.html
|—— contact.html
|—— index.html

The example shows three different files stored in one folder. HTML files are often stored in the same folder. If the browser is currently displaying index.html it also knows that about.html and contact.html are in the same folder, allowing use to link web pages together using a relative path. 
Example:
<a href="./contact.html">Contact</a>

In the above example, the anchor tag is used with a relative path to link to a file in the same folder. On the web page, "Contact" will appear as a hyperlink. 

A relative path is a filename that shows to a local file versus an absolute path which would pull a URL from an outside source like https://www.codecademy.com/learn/learn-html which is stored in a different folder. 

The "./" in "./index.html" tells the browser to look for the file in the current folder. 