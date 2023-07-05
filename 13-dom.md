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
- 
