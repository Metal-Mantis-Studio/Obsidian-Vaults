XPATH stands for XML Path Language and is used to navigate through elements and attributes in an XML document i.e. a webpage by navigation nodes. 
[XPATH Syntax](https://www.w3schools.com/xml/xpath_syntax.asp)
[XPATH Axes](https://www.w3schools.com/xml/xpath_axes.asp)

`use` - This will target any `<use>` elements within the document
`div/svg/use` - This will target any `<use>` elements which are direct descendants of a `div/svg` set of elements.
`div//use` - This will target any `<use>` elements which is a descendant of a div with any/no element descendants inbetween
`.` - Selects the current node
`..` - Selects the parent of the current node
`@` - Selects attributes i.e. title[@lang="en"] will select all `<title>` elements with a lang tag of "en"
`/use[1]` - Selects the first element
`/use[last()]` - Selects the last
`/use[last()-1]` - Selects the one before last
`/use[position()<3]` - Selects the first 2 `<use>` elements  