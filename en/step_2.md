## Your page

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Create the page you'll add your pictures, text, and videos to.
</div>
<div>
Image, gif or video showing what they will achieve by the end of the step. ![](images/image.png){:width="300px"}
</div>
</div>

--- task ---

If you're using Trinket in your browser, open [the template](#) and remix it. If you're wokring on your computer, download [the starter files](#), unzip them, and open them in your editor of choice.

--- /task ---

--- task ---

In `index.html` create a `div` with a background colour and set width. Then use CSS to centre it on the webpage. You can find some useful reminders of how to do this below.

**Choose:** Choose your background colour. You can find a list on [this page](https://www.w3schools.com/colors/colors_names.asp).

--- save ---

**Test:** view `index.html` to see the page layout.

--- /task ---

### Tools for making your page

--- collapse --- 
---
title: The `div` tag
---

A `div` is an invisible rectangle, with no width or height unless you give it one — either with CSS or by putting something inside it, which the `div` will grow to hold.

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