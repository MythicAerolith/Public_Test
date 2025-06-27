# Public_Test
Test for practicing repositories and collaboration 

LANGUAGE NOTES



HTML (Hypertext Markup Language): determines how a webpage looks and is formatted, content  & layout, create the basic structure of website

CSS: satatic programming language, styling and look, popular sheet style language (colors, fonts, layout, responsive fts), make more visually appealing

JavaScript: Interactive Elements, allows you to change both CSS and HTML elements on web after site has been loaded, ability to add animations,
embedded video media

to focus on improving FRONT-END elements of website, the most important languages to learn include, HTML5, CSS3, Bootstrap, and Javascript
for BACK-END, use Python, Ruby, and PHP

Markup Language- a computer language that defines the  structure and presentation of raw text
HyperText- text displayed on computer or device that provides access to other text through hjyperlinks


                                                                HTML
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


