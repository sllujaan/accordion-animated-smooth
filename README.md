# Team List (Animated)

![image](https://user-images.githubusercontent.com/31973579/159147603-c5d33f72-f0f7-474f-9e4b-3fc144e4cc25.png)

![image](https://user-images.githubusercontent.com/31973579/159147679-97f1849c-dd17-431a-a8b9-1b0f4f184e28.png)

![image](https://user-images.githubusercontent.com/31973579/159147636-ae926538-68ab-4ae0-bc7a-a4368590206b.png)

![image](https://user-images.githubusercontent.com/31973579/159147711-8d777ebf-52c3-4193-9fbd-41a02478887c.png)

# Installation

**For Commonjs & ESModules:**

```js
// in commonjs & ESModules
import { AccordionAnimated, AccordionItem } from "./accordion-animated.js";
// or
// in commonjs
const { AccordionAnimated, AccordionItem } = require("./accordion-animated.js");
```

**In Plain Javascript:**

```html
<!-- in html file -->
<head>
  ...
  <script src="./accordion-animated.js"></script>
  ...
</head>
<body>
  ...
  <script type="text/javascript">
    // code
  </script>
</body>
```

# Use

```html
<!-- in html file -->
<head>
  ...
  <style>
    .container {
        background-color: white;
        width: 100%;
        height: 100%;
    }
  </style>
</head>
<body>
  <div class="container"></div>
  ...
</body>
```

```js
// in script tag or index.js file

// retrieve the target element
const container = document.querySelectorAll(".container")[0];

// create an array for the list items
const accordionItems = [];

// create new list item and push it in the accordionItems array previously create.
accordionItems.push(
  new AccordionItem({
    name: "Lorem ipsum 3",
    nameColor: "black",
    title: "Title here",
    titleColor: "gray",
    iconColor: "black",
    imageUrl: "profile_user.jpg",
    hoverColor1: "#f4c7b2",
    hoverColor2: "#dedbe2",
    description: "<p>html description<p>",
    descriptionColor: "black",
    borderColor: "gray",
    shadowColorRGB: "1 1 1",
  })
);

// add some more items
accordionItems.push(
  new AccordionItem({
    ...
  })
);
accordionItems.push(
  new AccordionItem({
    ...
  })
);


// now initialize the List 
new AccordionAnimated({
  target: container,
  items: accordionItems
});


```




## [Click Here to See Live Demo](https://sllujaan.github.io/accordion-animated-smooth/)🚀
