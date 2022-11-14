## Learn CSS - Flexbox


### Flexbox is designed for one-dimensional content. Explain what this means. 
It is meant for items that are either single row or single column

### Explain the difference between the main axis and cross axis.
The main axis is the one set by your flex-direction property. If that is row your main axis is along the row, if it is column your main axis is along the column.
The cross axis runs in the other direction to the main axis, so if flex-direction is row the cross axis runs along the column.

### How can using certain properties of flexbox negatively impact accessibility?

You should be cautious when using any properties that reorder the visual display away from how things are ordered in the HTML document, as it can negatively impact accessibility. This is important to understand as the logical order is the order that a screen reader will read out the content, and anyone navigating using the keyboard will follow.

[flexbox](https://web.dev/learn/css/flexbox/)


[CSS Layout - Flexbox](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)



### What are some advantages of using flexbox over float?
Flexbox is responsive and mobile-friendly. Flex container's margins do not collapse with the margins of its content. We can easily change the order of elements on our webpage without even making changes in HTML.

### How does this topic connect with your long term goals?
Creating sharp well built web pages is absolutely a goal of mine, using flex box helps me meet those goals, and do so more efficiently.

Bookmark and Review
[Learn CSS - Layout](https://web.dev/learn/css/layout/)
Gives a good overview of when to use flex vs grid. 