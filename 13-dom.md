# Advanced DOM and Events

### 6/30/23

#### DOM API Organization Breakdown
![DOM API Organization](images/13-dom/dom-api-organization.png)

- To select the entire html document of a webpages, select the documentElement. (Just document alone is not a real dom element, so it is not enough to select.)
- for documentElement, head, and body, no additional selector is needed
![alt](images/13-dom/2023-06-30-8.png)

#### Creating and Inserting Elements
- prepend will add the new element as the first child of the parent element you're adding to
- append will add as last child of the specified parent element
- prepend and append can also be used to move elements to first or last child positions (not just insert them)
- this means that you can't have duplicates of an element by both prepending and appending it
- as a workaround, to insert it more than once, clone the element and its children with cloneNode
![alt](images/13-dom/2023-06-30-9.png)
- before and after insert the new element as a sibling of the specified element

### 7/5/23

- using the style method to apply new styles to an element in js automatically creates inline styles in the html (rather than a separate style in the css file)
- to log style info to the console, the style must be applied as in-line (can't pull from stylesheet)
- Use "getComputedStyle" to pull the style from the stylesheet. The computed style refers to the actual style, as it appears on the page.
![alt](images/13-dom/2023-07-05-01.png)
- getComputedStyle returns a string, so use Number.parseFloat to convert back to a number when manipulating the style.
![alt](images/13-dom/2023-07-05-02.png)
- the documentElement (described above) accesses the root element, so to change a CSS variable's property, first access the root, where CSS variables are stored
- the two inputs to the setProperty method are 1- which property to set, and 2- what to set it to (it's new value)
- 
