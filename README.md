# DOM
The Document Object Model (DOM) is a cross-platform and language-independent interface that treats an XML or HTML document as a tree structure wherein each node is an object representing a part of the document. The DOM represents a document with a logical tree. Each branch of the tree ends in a node, and each node contains objects. DOM methods allow programmatic access to the tree; with them one can change the structure, style or content of a document. Nodes can have event handlers attached to them. Once an event is triggered, the event handlers get executed.
The principal standardization of the DOM was handled by the World Wide Web Consortium (W3C), which last developed a recommendation in 2004. WHATWG took over the development of the standard, publishing it as a living document. The W3C now publishes stable snapshots of the WHATWG standard.
In HTML DOM (Document Object Model), every element is a node:

- A document is a document node.
- All HTML elements are element nodes.
- All HTML attributes are attribute nodes.
- Text inserted into HTML elements are text nodes.
- Comments are comment nodes.[Wikipedia](https://en.wikipedia.org/wiki/Document_Object_Model).

[![DOM](https://upload.wikimedia.org/wikipedia/commons/5/5a/DOM-model.svg)](https://en.wikipedia.org/wiki/Document_Object_Model)

## Get HTML Elements in Javascript:

- Using ID: `document.getElementById("id")`
- Using Class: `document.getElementsByClassName("class")`
- Using Tag: `document.getElementsByTagName("tag")`
- Using Query Selector: `document.querySelector("selector")`
- Using Query Selector All: `document.querySelectorAll("selector")`

```javascript
// Get element by ID
let element = document.getElementById("ID_FOR_ELEMENT"); // This will return the element with the ID "ID_FOR_ELEMENT" ONLY ONE ELEMENT.
let elements = document.getElementsByClassName("CLASS_FOR_ELEMENT"); // This will return all elements with the class "CLASS_FOR_ELEMENT" as HTMLCollection.
let elements = document.getElementsByTagName("TAG_FOR_ELEMENT"); // This will return all elements with the tag "TAG_FOR_ELEMENT" as HTMLCollection.
let element = document.querySelector("SELECTOR_FOR_ELEMENT"); // This will return the first element that matches the selector "SELECTOR_FOR_ELEMENT" ONLY ONE ELEMENT.
let elements = document.querySelectorAll("SELECTOR_FOR_ELEMENT"); // This will return all elements that matches the selector "SELECTOR_FOR_ELEMENT" as NodeList.
```

## HTMLCollection:
The HTMLCollection interface represents a generic collection (array-like object similar to arguments) of elements (in document order) and offers methods and properties for selecting from the list.[MDN](https://developer.mozilla.org/en-US/docs/Web/API/HTMLCollection).

## NodeList:
The NodeList interface represents a collection of nodes. The nodes can be accessed by index numbers. The items in the NodeList are accessible via an integral index, starting from 0.[MDN](https://developer.mozilla.org/en-US/docs/Web/API/NodeList).

## Loop through HTMLCollection or NodeList:
```javascript
// Loop through HTMLCollection or NodeList
let elements = document.getElementsByClassName("CLASS_FOR_ELEMENT");
for (let item of elements) {
    // Do something with item
}
// OR
Array.from(elements).forEach(item => {
    // Do something with item
});
```

## Some Important Methods:
- [Get HTML Element Attributes in Javascript](#get-html-element-attributes-in-javascript).
- [Set HTML Element Attributes in Javascript](#set-html-element-attributes-in-javascript).
- [Remove HTML Element Attributes in Javascript](#remove-html-element-attributes-in-javascript).
- [Get HTML Element Style in Javascript](#get-html-element-style-in-javascript).
- [Set HTML Element Style in Javascript](#set-html-element-style-in-javascript).
- [Get HTML Element Content in Javascript](#get-html-element-content-in-javascript).
- [Set HTML Element Content in Javascript](#set-html-element-content-in-javascript).
- [Get HTML Element Text in Javascript](#get-html-element-text-in-javascript).
- [Set HTML Element Text in Javascript](#set-html-element-text-in-javascript).
- [Get HTML Element Class in Javascript](#get-html-element-class-in-javascript).
- [Set HTML Element Class in Javascript](#set-html-element-class-in-javascript).
- [Add HTML Element Class in Javascript](#add-html-element-class-in-javascript).
- [Remove HTML Element Class in Javascript](#remove-html-element-class-in-javascript).
- [Toggle HTML Element Class in Javascript](#toggle-html-element-class-in-javascript).
- [Check HTML Element Class in Javascript](#check-html-element-class-in-javascript).
- [Get HTML Element Children in Javascript](#get-html-element-children-in-javascript).
- [Get HTML Element Parent in Javascript](#get-html-element-parent-in-javascript).
- [Get HTML Element Siblings in Javascript](#get-html-element-siblings-in-javascript).
- [Get HTML Element Next Sibling in Javascript](#get-html-element-next-sibling-in-javascript).
- [Get HTML Element Previous Sibling in Javascript](#get-html-element-previous-sibling-in-javascript).
- [Get HTML Element First Child in Javascript](#get-html-element-first-child-in-javascript).
- [Get HTML Element Last Child in Javascript](#get-html-element-last-child-in-javascript).
- [Get HTML Element Width in Javascript](#get-html-element-width-in-javascript).
- [Get HTML Element Height in Javascript](#get-html-element-height-in-javascript).
- [Get HTML Element Position in Javascript](#get-html-element-position-in-javascript).
- [Get HTML Element Position Top in Javascript](#get-html-element-position-top-in-javascript).
- [Get HTML Element Position Left in Javascript](#get-html-element-position-left-in-javascript).
- [Get HTML Element Position Right in Javascript](#get-html-element-position-right-in-javascript).
- [Get HTML Element Position Bottom in Javascript](#get-html-element-position-bottom-in-javascript).
- [Get HTML Element Position Width in Javascript](#get-html-element-position-width-in-javascript).
- [Get HTML Element Position Height in Javascript](#get-html-element-position-height-in-javascript).
- [Get HTML Element Position X in Javascript](#get-html-element-position-x-in-javascript).
- [Get HTML Element Position Y in Javascript](#get-html-element-position-y-in-javascript).
- [Get HTML Element Position Center in Javascript](#get-html-element-position-center-in-javascript).


## Get HTML Element Attributes in Javascript:
```javascript
// Get element attributes
let element = document.getElementById("ID_FOR_ELEMENT");
let attribute = element.getAttribute("ATTRIBUTE_NAME");
```
<hr>

## Set HTML Element Attributes in Javascript:
```javascript
// Set element attributes
let element = document.getElementById("ID_FOR_ELEMENT");
element.setAttribute("ATTRIBUTE_NAME", "ATTRIBUTE_VALUE");
```

<hr>

## Remove HTML Element Attributes in Javascript:
```javascript
// Remove element attributes
let element = document.getElementById("ID_FOR_ELEMENT");
element.removeAttribute("ATTRIBUTE_NAME");
```

<hr>

## Get HTML Element Style in Javascript:
```javascript
// Get element style
let element = document.getElementById("ID_FOR_ELEMENT");
let style = element.style;
```

<hr>

## Set HTML Element Style in Javascript:
```javascript
// Set element style
let element = document.getElementById("ID_FOR_ELEMENT");
element.style = "STYLE";
```

<hr>

## Get HTML Element Content in Javascript:
```javascript
// Get element content
let element = document.getElementById("ID_FOR_ELEMENT");
let content = element.innerHTML;
```

<hr>

## Set HTML Element Content in Javascript:
```javascript
// Set element content
let element = document.getElementById("ID_FOR_ELEMENT");
element.innerHTML = "CONTENT";
```

<hr>

## Get HTML Element Text in Javascript:
```javascript
// Get element text
let element = document.getElementById("ID_FOR_ELEMENT");
let text = element.innerText;
```

<hr>

## Set HTML Element Text in Javascript:
```javascript
// Set element text
let element = document.getElementById("ID_FOR_ELEMENT");
element.innerText = "TEXT";
```

<hr>

## Get HTML Element Class in Javascript:
```javascript
// Get element class
let element = document.getElementById("ID_FOR_ELEMENT");
let class = element.className;
```

<hr>

## Set HTML Element Class in Javascript:
```javascript
// Set element class
let element = document.getElementById("ID_FOR_ELEMENT");
element.className = "CLASS";
```

<hr>

## Add HTML Element Class in Javascript:
```javascript
// Add element class
let element = document.getElementById("ID_FOR_ELEMENT");
element.classList.add("CLASS");
```

<hr>

## Remove HTML Element Class in Javascript:
```javascript
// Remove element class
let element = document.getElementById("ID_FOR_ELEMENT");
element.classList.remove("CLASS");
```

<hr>

## Toggle HTML Element Class in Javascript:
```javascript
// Toggle element class
let element = document.getElementById("ID_FOR_ELEMENT");
element.classList.toggle("CLASS");
```

<hr>

## Check HTML Element Class in Javascript:
```javascript
// Check element class
let element = document.getElementById("ID_FOR_ELEMENT");
let hasClass = element.classList.contains("CLASS");
```

<hr>

## Get HTML Element Children in Javascript:
```javascript
// Get element children
let element = document.getElementById("ID_FOR_ELEMENT");
let children = element.children;// This will return all children of the element as HTMLCollection.
```

<hr>

## Get HTML Element Parent in Javascript:
```javascript
// Get element parent
let element = document.getElementById("ID_FOR_ELEMENT");
let parent = element.parentElement;// This will return the parent of the element.
```

<hr>

## Get HTML Element Siblings in Javascript:
```javascript
// Get element siblings
let element = document.getElementById("ID_FOR_ELEMENT");
let siblings = element.parentElement.children;// This will return all siblings of the element as HTMLCollection.
```

<hr>

## Get HTML Element Next Sibling in Javascript:
```javascript
// Get element next sibling
let element = document.getElementById("ID_FOR_ELEMENT");
let nextSibling = element.nextElementSibling;// This will return the next sibling of the element.
```

<hr>

## Get HTML Element Previous Sibling in Javascript:
```javascript
// Get element previous sibling
let element = document.getElementById("ID_FOR_ELEMENT");
let previousSibling = element.previousElementSibling;// This will return the previous sibling of the element.
```

<hr>

## Get HTML Element First Child in Javascript:
```javascript
// Get element first child
let element = document.getElementById("ID_FOR_ELEMENT");
let firstChild = element.firstElementChild;// This will return the first child of the element.
```

<hr>

## Get HTML Element Last Child in Javascript:
```javascript
// Get element last child
let element = document.getElementById("ID_FOR_ELEMENT");
let lastChild = element.lastElementChild;// This will return the last child of the element.
```

<hr>

## Get HTML Element Width in Javascript:
```javascript
// Get element width
let element = document.getElementById("ID_FOR_ELEMENT");
let width = element.offsetWidth;// This will return the width of the element.
```

<hr>

## Get HTML Element Height in Javascript:
```javascript
// Get element height
let element = document.getElementById("ID_FOR_ELEMENT");
let height = element.offsetHeight;// This will return the height of the element.
```

<hr>

## Get HTML Element Position in Javascript:
```javascript
// Get element position
let element = document.getElementById("ID_FOR_ELEMENT");
let position = element.getBoundingClientRect();// This will return the position of the element.
```

<hr>

## Get HTML Element Position Top in Javascript:
```javascript
// Get element position top
let element = document.getElementById("ID_FOR_ELEMENT");
let positionTop = element.getBoundingClientRect().top;// This will return the position top of the element.
```

<hr>

## Get HTML Element Position Left in Javascript:
```javascript
// Get element position left
let element = document.getElementById("ID_FOR_ELEMENT");
let positionLeft = element.getBoundingClientRect().left;// This will return the position left of the element.
```

<hr>

## Get HTML Element Position Right in Javascript:
```javascript
// Get element position right
let element = document.getElementById("ID_FOR_ELEMENT");
let positionRight = element.getBoundingClientRect().right;// This will return the position right of the element.
```

<hr>

## Get HTML Element Position Bottom in Javascript:
```javascript
// Get element position bottom
let element = document.getElementById("ID_FOR_ELEMENT");
let positionBottom = element.getBoundingClientRect().bottom;// This will return the position bottom of the element.
```

<hr>

## Get HTML Element Position Width in Javascript:
```javascript
// Get element position width
let element = document.getElementById("ID_FOR_ELEMENT");
let positionWidth = element.getBoundingClientRect().width;// This will return the position width of the element.
```

<hr>

## Get HTML Element Position Height in Javascript:
```javascript
// Get element position height
let element = document.getElementById("ID_FOR_ELEMENT");
let positionHeight = element.getBoundingClientRect().height;// This will return the position height of the element.
```

<hr>

## Get HTML Element Position X in Javascript:
```javascript
// Get element position x
let element = document.getElementById("ID_FOR_ELEMENT");
let positionX = element.getBoundingClientRect().x;// This will return the position x of the element.
```

<hr>

## Get HTML Element Position Y in Javascript:
```javascript
// Get element position y
let element = document.getElementById("ID_FOR_ELEMENT");
let positionY = element.getBoundingClientRect().y;// This will return the position y of the element.
```

<hr>

## Get HTML Element Position Center in Javascript:
```javascript
// Get element position center
let element = document.getElementById("ID_FOR_ELEMENT");
let positionCenter = element.getBoundingClientRect().center;// This will return the position center of the element.
```

<hr>
