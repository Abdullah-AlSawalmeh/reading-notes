# Layout
Controlling the position of elements

CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.

Block-level elements start on a new line Examples include: <h1> <p> <ul> <li>
Inline elements flow in between surrounding text Examples include: <img> <b> <i>

# Controlling the Position of El ements

CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the position property in CSS. You can also float elements using the float property.

1. Normal flow Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one. Even if you specify the width of the boxes and there is space for two elements to sit side-byside, they will not appear next to each other. This is the default behavior (unless you tell the browser to do somethingelse)

2. Relative Positioning This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. This does not affect the position of surrounding elements; they stay in the position they would be in in normal flow.

3. Absolute positioning This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements (as they simply ignore the space it would have taken up). Absolutely positioned elements move as users scroll up and down the page.

# block in css
What is a block in CSS?

A block-level element always starts on a new line and takes up the full width available (stretches out to the left and right as far as it can). The <div element is a block-level element. ... <div


# What is inline-block in CSS?

inline-block It's formatted just like the inline element, where it doesn't start on a new line. BUT, you can set width and height values. block The element will start on a new line and occupy the full width available. And you can set width and height values span is the standard inline element. An inline element can wrap some text inside a paragraph <span like this </span without disrupting the flow of that paragraph. The a element is the most common inline element, since you use them for links.