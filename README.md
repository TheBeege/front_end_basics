# Front End Basics

## Get an Editor
First, download and install [Brackets](https://brackets.io). Brackets is an editor for web development. Once you've installed it, if you type in some HTML and click the lightning bolt on the top right, it will show your page in chrome and auto refresh it when you make changes.


## HTML

### Concepts
Let's go over HTML. It's short for HyperText Markup Language. It is a markup language, not a programming language, which means you can't do logic with it. Hypertext is very literal - it's a super version of text. When you look at a web page, you're actually looking at a text document. Your browser talks to the server and says, "please give me the text document at this location." Things like images, videos, etc are just referenced from the text document. You can see an example of this if you right click an image on a web page and hit Inspect. HTML is just code written around text to make it "hyper". At the highest level, that's HTML conceptually.

Getting deeper, HTML is a way to give content on a web page some amount of (ideally semantic) structure. Portions of text or other resources are organized into sections. Some elements are organized into headers, paragraphs, and footers. Portions of content are identified as belonging to a certain "class" of content or given a unique ID. HTML can also give a website useful metadata, like a page title, search keywords, what language the page is in, and more. HTML can also mark what positions among text that additional content should appear like images and videos, and it marks certain bits of content as links to other pages.

### Tags
Let's get even deeper. HTML is composed of "tags". Tags are basically information between less than and greater than signs <>. Some tags are composed of a start tag and an end tag. An end tag has a slash after the less than sign. For example:

```html
<p>This is a paragraph.</p>
```

The <p> tag has a start and end, the end being </p>. This means that the stuff between the start and end is considered a paragraph, and the browser will understand this. A portion of HTML, from start tag to end tag and including information in between is called an "element". Not all tags have a start and end, meaning that the tag itself could be the entire element. Tags that don't have a corresponding end are self-terminating. Here's an example:

```html
<img />
```

This is an img tag that has no corresponding end tag, which is shown by the slash before the greater than sign.

HTML elements can have other elements inside them. See this example:

```html
<p>You'll learn HTML <strong>really</strong> fast.</p>
```

Here, we have a strong element inside a paragraph element. This is a major concept of HTML: elements can contain other elements. This is necessary for creating pages and helpful in a text editor. To keep things manageable, you can usually visually collapse tags in an editor to keep the text in front of you minimal. This helps keep things from being distracting or overwhelming, and it makes scrolling through large pages faster.

### Attributes
One last thing about HTML. A tag can have "attributes". These are simple key value pairs, like class="blue-text", where the key is before an equals symbol and the value comes after it, often in quotes. An image tag is the classic example:

```html
<img src="https://i.kym-cdn.com/entries/icons/original/000/000/091/TrollFace.jpg" />
```

This will get the image at the address for the "src" attribute, and show it at the img element's location on the page. Some tags have special attributes like img's src attribute, but there are also some universal attributes. You'll learn these when you dive more into HTML.

### Addresses and Paths
A quick note about addresses in web pages.

#### Fully Qualified Addresses
In the example above, we use a "fully qualified" address - it's an address that you could just plug into your browser and expect to work. There are also absolute and relative paths.

#### Relative Paths
If you had a page at example.com/mypage.html, and your image source was "my_image.jpg", it would look for an image at example.com/my_image.jpg. This is a relative path. If your page was at example.com/folder/page.html and used "images/my_image.jpg" as the source, it would look for an image at example.com/folder/images/my_image.html.

#### Absolute Paths
Alternatively, you could use "/my_image.html". This is an absolute path. The leading slash tells it to start looking for the image from the main domain. For example, if we had a page at example.com/pages/index.html, and our image source was "/images/lol.png", it would look for an image file at example.com/images/lol.png.

### You're Ready to Dive In!
At this point, you're ready to learn the nitty gritty of HTML. I strongly recommend w3schools. [Check out their HTML tutorial](https://www.w3schools.com/html/)

## CSS
