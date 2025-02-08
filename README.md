# Uncommon HTML Bug: Incorrect textContent Access

This repository demonstrates an uncommon bug related to accessing the `textContent` property of an HTML div element that contains nested elements.  The `textContent` property only returns the text directly within the element, not the text content of its children.

## Bug Description:
The code attempts to extract all text within a div element using `textContent`. However, if the div contains nested elements (like a paragraph tag `<p>` in this case), only the text directly within the div is returned, ignoring text within the nested elements. This can lead to unexpected results and incorrect data extraction.

## Bug Solution:
The solution involves iterating through all child nodes of the div and concatenating their text content to get the complete text from the div and all its children.