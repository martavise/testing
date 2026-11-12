# CSS
## Selectors
They select the element to which apply the style.   
`*` is the universal selector and it will select elements of every type (as in the whole document)   
```
* {
  color: purple;
}
```
There are **type selectors** which will select all elements of the given element type, and their syntax is just the name of the element

```
div {
  color: white;
}
```  
**Class selectors** apply to element inside the given class (in the html the class is marked as an attribute)

```
html:
<div class="alert-text">Please agree to our terms of service.</div>   

css:
.alert-text {
  color: red;
}
```  
**ID selectors** are similar to class ones, but an element can only have one ID. An ID cannot be repeated on a single page and should not contain any whitespace. 
```
html:
<div id="title">My Awesome 90's Page</div>

css:
#title {
  background-color: red;
}
```

Selectors can be grouped with a comma
```
.read,
.unread {
  color: white;
  background-color: black;
}
```

Gli elementi possono avere più attributi, quando si vuole essere più specifici su quali combinazioni si vuole lavorare, è possibile concatenare i selectors in css con punti. (non si possono concatenare type selectors)
```
<div>
  <div class="subsection header">Latest Posts</div>
  <p class="subsection" id="preview">
    This is where a preview for a post might go.
  </p>
</div>


.subsection.header {
  color: red;
}

.subsection#preview {
  color: blue;
}

```

## Some properties
#### color
- **color property** sets an element’s text color
- **background-color** sets the background color of an element
```
p {
  /* hex example: */
  color: #1100ff;
}

p {
  /* rgb example: */
  color: rgb(100, 0, 127);
}

p {
  /* hsl example: */
  color: hsl(15, 82%, 56%);
}
```
#### text
- **font-family** can be a single value or a comma-separated list of values that determine what font an element uses  
- **font-size** will set the size of the font. When giving a value to this property, the value should not contain any whitespace, e.g. font-size: 22px has no space between “22” and “px”
- **font-weight** affects the boldness of text, assuming the font supports the specified weight. This value can be a keyword, e.g. font-weight: bold, or a number between 1 and 1000
- **text-align** will align text horizontally within an element, and you can use the common keywords you may have come across in word processors as the value for this property, e.g. text-align: center
#### images
- aggiusto altezza e larghezza se non voglio usare quelle del file (usando auto su uno degli attributi, ne mantengo le proporzioni)
```
img {
  height: auto;
  width: 500px;
}
```

## Integrare CSS in HTML
1. *internal* Si può fare direttamente nel file html con il divisore `<style></style>`
2. *inline* Direttamente aggiungendo gli attributi all'elemento 
```
<div style="color: white; background-color: black;">...</div>
```
3. *external* Consigliato per avere html più pulito e riutilizzare CSS su più pagine del sito. Si fa un file css separato che viene richiamato nella head dell'html
```
<head>
  <link rel="stylesheet" href="styles.css">
</head>
```