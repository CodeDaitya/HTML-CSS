# Hypertext Markup Language

HTML, Hypertext Markup Language gives structure and meaning to the content by defining that content in web page. These can be parahraphs,headings,  
images etc. It provides us with the ability to put some content on the internet in the form of webpages, it doesn't define any of the display rules 
for how the content will be displayed. It's just throw the raw data of all the different kinds according to their definition.

## HTML Terms

### Elements

Elements are the designators that define the structure and content of object within a page. It is identified by the two enclosing angled brackets,
`< >`. The most commonly used HTML elements are the heading elements, `h1` through `h6` differing in level, and the paragraph element, `p`. Other
elements include `a`, `div`, `span` etc.

### Tags

A _tag_ is an element enclosed in the two angled brackets, like `<h1>` tag for first level heading element. Tags commonly occur in pair of opening
and closing tags. The closing tag looks a little different from the opening tag, like `</h1>` closing tag for the first level heading element.

The content that falls between the pair of tags, is that content of that element, like in 
```html
<h1> This is a heading
</h1>
```
"This is a heading" is the content of element the `h1`.

#### Self-enclosing Elements

Some elements have all their content within a single tag. They don't need a closing tag and thus are _self-closing_.

```html
<br> <embed> <hr> <img> <input> <wbr>
<meta> <param> <source> <link>
```

### Attributes

Attributes are the properties used to provide additional information about an element. An attriute is defined within the opening tag after the name
of the element. It is defined with it's name followed by an `=` sign followed the value for that attribute in double quotes.

```html
<a href="somelink.com">Link</a>
```

Here, `href` is an attribute that is used to define hyperlink to the anchor tag `<a>` content, and "somelink.com" is the value it is linked to.  

### Document Structure

An HTML document is a plain text document save with ab `.html` file extension. The document is authored in an editor.  

All HTML documents has a required structure that includes the following declaration and elements `<!DOCTYPE>, <html>, <head>, and <body>`.

`<!DOCTYPE hmtl>` informs the web browser which version of HTML is being used in the very beginning of the document. Simply writing `html` without
any version information signifies that latest html version is being used.  

`<html>` signifies the beginning of the document.  

`<head>` inside <html> identifies the top of the document including any metadata. It may include document title, or any other beneficial metadata.  

`<body>` contains all the content visible in the web page.  

```html
<!DOCTYPE html>
<html lang="en">
	<head>
		<title>Hello World</title>
		<meta charset="utf-8">
	</head>
	<body>
		<h1>Hello World</h1>
		<p>This is a web page</p>
	</body>
</html>
```
