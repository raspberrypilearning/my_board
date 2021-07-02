## Your page

--- task ---

If you're using Trinket in your browser, open [the template](https://trinket.io/html/00ad891a2c){:target="_blank"} and remix it. If you're working on your computer, download [the starter files](rpf.io/p/en/my_board-get), unzip them, and open them in your editor of choice.

--- /task ---

--- task ---

In `index.html` create a `div` with a background colour and set width. Then use CSS to centre it on the webpage. You can find some useful reminders of how to do this below.

**Choose:** Choose your background colour. You can find a list on [this page](https://www.w3schools.com/colors/colors_names.asp){:target="_blank"}.

--- collapse --- 
---
title: The div tag
---

A `div` is an invisible rectangle. It has no width or height unless you do something to give them to it. You can give a `div` width and height with the CSS `width` and `height` properties. You can also put another element inside the `div`, and the `div` will grow to hold that element.

```html
    <div>
        <!-- Whatever you want to put in your div -->
    </div>
```

--- /collapse ---

--- collapse ---
---
title: Assigning CSS rules with classes
---

You can use a class on a HTML element to connect it with a set of CSS rules, like this:

```html
    <p class="my_class">
        Here is the text of a paragraph.
    </p>
```

```css
.my_class{
    /* CSS rules go here */
}
``` 

--- /collapse ---

--- collapse ---
---
title: Setting background colour with CSS
---

You can set the background colour of an element with the `background-color` property:

```css
.my_class{
    background-color: green;
}
```

--- /collapse ---

--- collapse ---
---
title: Centring elements with CSS
---

You can centre a HTML element inside its parent (the element which contains it) by setting the `margin-left` and `margin-right` of the element to `auto`:

```css
.my_class{
    margin-left: auto;
    margin-right: auto;
}
```

--- /collapse ---

--- collapse ---
---
title: Setting width and height with CSS
---

You can set the `width` and `height` properties of a HTML element:

```css
.my_class{
    height: 150px;
    width: 200px;
}
```

--- /collapse ---

--- save ---

**Test:** view `index.html` to see the page layout.

--- /task ---

--- task ---

Give the container `div` the property `overflow: hidden`. This will make it grow around the grid elements you will set to `float` in the next step.

--- save ---

--- /task ---
