
# Web Development Practice and Notes (Using [The Odin Project](https://www.theodinproject.com/))

### This will be my web development notes along with dates about what I have learned to show my progression, so follow along with me on my journey in learning full stack development!


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
- Please reference [working_with_text: index.html][test_index.html] 

### Lists

- 

### Links and Images

- 

## TO DO:

### Continue with the Links and Images Assignment on "The Odin Project" curriculum.

<!--- LINK REFERENCES --->
[html_index]: https://github.com/jonathan-mendoza1/webdev_prac/blob/main/html-boilerplate/index.html
[html_index2]: https://github.com/jonathan-mendoza1/webdev_prac/blob/main/html-boilerplate/index2.html
[text_index.html]: https://github.com/jonathan-mendoza1/webdev_prac/blob/main/working_with_text/index.html
[text_test.html]: https://github.com/jonathan-mendoza1/webdev_prac/blob/main/working_with_text/test.html