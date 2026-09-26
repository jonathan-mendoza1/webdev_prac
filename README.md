
# Web Development Practice and Notes (Using [The Odin Project](https://www.theodinproject.com/))

### This will be my web development notes along with dates about what I have learned to show my progression, so follow along with me on my journey in learning full stack development!

<br>

## September 25, 2026 - HTML Foundations

### Elements and Tags

- HTML elements and tags are some of the basic building blocks of an HTML document. An element generally consists of content wrapped in an opening tag and a closing tag. For example, a paragraph element uses an opening `<p>` tag and a closing `</p>` tag.
- Most HTML elements have both an opening and closing tag, but there are some void elements, such as `<br>` and `<img>`, that do not have closing tags because they cannot contain any content.
- For example:
    - `<p>` = opening tag
    - Hello, World! = content
    - `</p>` = closing tag
    - The entire thing = element

### HTML Boilerplate

- An HTML boilerplate is the basic structure that every HTML document starts with, and all html files use the `.html` extension.
- The homepage of a website is usually named `index.html`.
- `<!DOCTYPE html>` tells the browser that the document uses HTML5.
- The `<html>` element is the root element of the HTML document, and is accompanied by the `<lang>` attribute that specifies the language of the page, 
    - Example: `<html lang="en">` - This specifies that the HTML document is in English.
- The `<head>` element contains information about the webpage, but is not displayed on the page itself.
    - `<meta charset="UTF-8">` specifies the character encoding so special characters and symbols display correctly, and `<title>` sets the title displayed in the browser tab.
- The `<body>` element contains the content that is displayed on the webpage like headings, paragraphs, images, links, and lists.
- Please reference [html-boilerplate: index.html][html_index] to see the basic structure of an HTML file. 
- Please reference [html-boilerplate: index2.html][html_index2] to see the basic structure of an HTML file auto-filled by VS Code by typing `!` and pressing `Enter`.

### Working with Text

- The `<p>` element is used to create paragraphs. Simply putting text on separate lines in HTML does not create paragraphs since browsers will collapse whitespace and line breaks in HTML into a single space. Use separate `<p>` elements when there should be separate paragraphs on the page.
- There are multiple types of headings in HTML with `<h1>` representing the highest level heading and `<h6>` representing the lowest. These levels create a hierarchy for the content on a webpage with `<h1>` usually being used for the main heading on a page, and lower levels being used for subsections.
- The `<strong>` element makes text appear bold and gives it semantic importance. This semantic importance can also assist other technologies, like text readers, to emphasize the importance of the content inside the element. However, only use this element when the text is important rather than just wanting to make the text bold. CSS will be better when the text just has to be bold on the page.
- The `<em>` element makes text appear italicized and gives it semantic emphasis. This also assist other technolgies, like text readers, to emphazise the content inside the element. Again, only use this element when the text needs emphasis, and not when it only has to be italicized. CSS will be better for this when the text just has to be italicized.
- Nesting means placing an HTML element inside another element. The element containing another element is called the parent,and the element inside the parent is called the child. If there is another element in the same nesting level as the child, those elements are called siblings.
- HTML comments allow for notes to be added into the code, but will not be displayed on the page. These comments are written like: `<!-- This is an HTML comment -->`.
- Please reference [working_with_text: index.html][text_index] for notes on these elements and how they work.
- Please reference [working_with_text: test.html][text_test] for my practice using these elements and creating my very first "blog post".

### Lists

- There are multiple types of lists that can be used in an HTML file, but for this section, only unordered and ordered lists are needed.
- The `<ul>` element creates and unordered list, like a grocery shopping list, where the order of information is not important. Each item in the list is created with the `<li>` element.
- The `<ol>` element creates and ordered list, like a recipe with steps, where the order of information is important. For example, an ordered list with 10 items would number each item, top to bottom, from 1-10. Again, each item in the list is created with the `<li>` element.
- Please reference [lists: index.html][lists_index] for notes on those elements and how they work.
- Please reference [lists: index.html][lists_prac] for my practice using these elements in different types of lists.

### Links and Images

#### Links:

- The `<a>` element creates links in the HTML file. These elements are accompanied by the `href` attribute to point at the destination of the link. These can be absolute or relative links.
    - Absolute links contain the complete URL to the destination of the resourse. For example, these can be `https://` links that are found on the address bar on the top bar of your browser. These normally include the scheme, domain, and path.
    - Relative links contain paths to other files within the same webpage like other pages on a website. For example, an "About" page on a website could be a linked by a relative link by writing `./pages/about.html`, given that the website has that file structure.
- The `<a>` element can also be accompanied by the `target` attribute, which determines how the link will open.
    - When the `target` value is set to `_blank`, the link will open a new tab in the browser. 
    - However, if the value is not specified or empty, the value will be defaulted to `_self` and the link will open within the same tab that is being used.
- The `<a>` element may also be accompanied by the `rel` attribute which describes the relation between the current page and the linked document.
    - When the `rel` value is set to `noopener`, this prevents the new page from accessing the original page that it was referenced from. Most modern browsers will automatically set this as the default value when the `target` value is set to `_blank`.
    - When the `rel` value is set to `noreferrer`, it works the same as `noopener`, but also prevents some details from the original page being passed onto the new page.

#### Images: 

- The `<img>` element allows for images to be displayed on the page. These elements are accompanied by the `src` attribute, which specifies the location for the image.
    - Both absolute and relative paths can be used for the `src` attribute to point at the location of the image that will be displayed on the page.
- The `<img>` element can also be accompanied by the `alt` attribute.
    - The provides alternate text to describe the image if the image cannot be loaded or displayed on the page.
    - This attribute also helps technologies, like text readers, to describe the image displayed on the page to visually impaired users.
    - Most images should have an appropriate `alt` attribute.
- The `<img>` element may also be accompanied by the `height` and `width` attributes which set the dimensions of the image on the page.
    - The `height` attribute sets the height of the image and the `width` attribute sets the width of the image, both using pixels as their values.
    - Specifying these dimensions are not necessary, but are typically better to have so images will not flash or overlap other elements on the page. It will also reserve that amount of space for the image on the page as it loads.

#### References:

- Please reference [links_and_images: index.html][l_and_i_index] for notes on how these links and images work in an HTML file.


<br>
<br>


<!--- LINK REFERENCES --->
[html_index]: https://github.com/jonathan-mendoza1/webdev_prac/blob/main/html-boilerplate/index.html
[html_index2]: https://github.com/jonathan-mendoza1/webdev_prac/blob/main/html-boilerplate/index2.html
[text_index]: https://github.com/jonathan-mendoza1/webdev_prac/blob/main/working_with_text/index.html
[text_test]: https://github.com/jonathan-mendoza1/webdev_prac/blob/main/working_with_text/test.html
[lists_index]: https://github.com/jonathan-mendoza1/webdev_prac/blob/main/lists/index.html
[lists_prac]: https://github.com/jonathan-mendoza1/webdev_prac/blob/main/lists/prac.html
[l_and_i_index]: https://github.com/jonathan-mendoza1/webdev_prac/blob/main/links_and_images/index.html