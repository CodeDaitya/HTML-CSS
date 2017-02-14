# Cascaded Style Sheet

CSS, Cascaded Style Sheet is a presentation language created to style the appearnace of the content. CSS define all the display style information
is applied on the HTML document to have different kinds of visual features and affects to the plain HTML element data. CSS can be used to define
things like color, size, position etc. for the desired portion in HTML.

## CSS Terms

### Selectors

Selectors designate exactly which element(s) within the HTML document to apply the style to. May include a combination of different qualifiers to
select unique elements depending on how specific the selection is suppossed to be.  

It generally targets an attribute value like `id` or `class` value, or target the type of element such as <h1> or <p>.  

Selectors are defined with the name of the selector followed by curly braces, `{ }` which enclose the style. 

```css
h1{....}
p{....}
```

### Properties

Properties determines style that will be applied to an element. It is defined inside the curly braces after the selector by it's name, followed by a
colon, `:`.

Properties define what kind of presentation an element will have vis-a-vis color, size, position, or some visual affects.

```css
h1{font-size:....}
p{color:....}
```

### Values

Values for every property is specified after the colon after the property name. The values specifies the exact property value for an element from a
set of possible values for that particular property.  

```css
h1{font-size: 63px;}
p{color: #fad65e;}
```  

## Selectors  

### Type Selectors  

Type selectors target elements by their element type. The specified style, in this case the style applies to all the instances of that element type
in the HTML document.

**CSS**  
```css
div{....}
```  

**HTML**  
```html
<div>..</div>
```  

### Class Selectors

Class selectors select an elements based on the value of their class attribute value. It is more specific as it selects a certain specific set of
elements in an HTML document whose value for class attribute is same as the class selector.  
It can be used to apply same style to different elements at once with the same class value.  
Classes in a CSS file are denoted with a leading period, `.`, followed by the class attribute value.  

**CSS**  
```css
.menu{....}
```  

**HTML**  
```html
<div class="menu">..</div>
<div class="menu">..</div>
```  

### ID Selectors  

This selector type even more specific as it only selects one unique element at time. It uses an `id` attribute value as a selector. `id` attribute
value can be used only once per page.  

The ID selector in a CSS file are denoted by a leading hash sign, `#`, followed by the `id` attribute value.  

**CSS**
```css
#id{....}
```  

**HTML**
```html
<div id="id">..</div>
```

## Referencing CSS  

In order to  apply the style defined in the external CSS file to our HTMl code, we need to reference the CSS file within the HTML document. The file
is refernced in the `head` element of the HTML document.  

Within the `<head>`, the `<link>` element is used to attach the CSS file with HTML. Their relationship is specified using the `rel` attribute with a
value `stylesheet`. `href` attribute is used to locate the CSS file in the filesystem.  

``html
<head>
	<link rel="stylesheet" href="style.css">
</head>
```  

In the above code, the CSS file exist in the directory as the HTML file called the Root directory. If it's present in some other directory, the
absolute path to that directory, or it's relative path can be used.  

```css
<head>
	<link rel="stylesheet" href="style/style.css">
</head>
```  

Above code references the CSS file in the sub-directory of the Root directory, style using it's path relative to the root directory.
