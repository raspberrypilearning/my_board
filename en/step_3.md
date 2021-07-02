## Your grid

--- task ---

Create a class to make all the items in your grid the same size. You'll also need to make them `float` to the left, so they form a grid.

--- collapse ---
---
title: Making a grid of elements with CSS
---

To make a grid of HTML elements with CSS, you will need to set a common height and width for all the elements, and set them to float to the left. For a neat layout, the width of an element in the grid should divide evenly into the width of the container (usually a `div`) you are placeing the elements into. For example, if the container `div` is 1200px wide, grid elements could be any of:

 + 600px
 + 400px
 + 300px

 Or even smaller, though things might start to get a little squashed!

```css
.my_grid_element{
    float: left;
    height: 400px;
    width: 400px;
}
```

--- /collapse ---

--- save --- 

--- /task ---

--- task ---

Add at least one image to your grid. You can find an image online, use one of the images included in the starter, or use one you already have. **Remember not to include photographs of yourself or your friends if you are going to publish the page online**.

[[[generic-get-picture-from-web]]]

[[[images-permissions-to-use]]]

--- collapse ---
---
title: Adding images to Trinket
---

To add an image to your Trinket project, first choose the Images section by selecting this icon.

![The image file icon](trinket_img.png)

Next, choose the "Image Library" button.

![The image library button](trinket_img_lib.png)

In the screen that opens, select "Upload New Image".

![The image upload button](trinket_img_upload_button.png)

Then drag the images you want to upload into the box that appears.

![The image upload box](trinket_img_upload_box.png)

--- /collapse ---

--- collapse ---
---
title: Including images in your webpage
---

The `img` tag is used to include pictures on a webpage. It has two attributes that must be set when doing so:

 + `src` — the source location of the image file, including the file name
 + `alt` — the alternative text description of the image, for users who rely on assistive tools to browse your site

 ```html
<img scr="my_dog.png" alt="A dog sitting in a garden.">
 ```

--- /collapse ---

--- save --- 

**Test:** view `index.html` to see your image(s).

--- /task ---

--- task ---

Add at least one paragraph of text to your grid. This could be a quote, an interesting fact, some song lyrics, or any other text you might want to include.

**Choose:** You can also include headings in a `div` with your paragraph, using the `h1` to `h6` tags.

--- collapse ---
---
title: Including paragraphs of text in your webpage
---

The `p` tag is used to add paragraphs of text to your webpage.

```html
<p> 
    Whatever text you want to add to your webpage.
</p>

<p> 
    Another paragraph of text you want to include.
</p>
```

--- /collapse ---

--- collapse ---
---
title: Styling text with CSS
---

You can use the `font-family` properity to make your text look different. The font families are:

  + <span style="font-family: cursive">cursive</span>
  + <span style="font-family: fantasy">fantasy</span>
  + <span style="font-family: monospace">monospace</span>
  + <span style="font-family: sans-serif">sans-serif</span>
  + <span style="font-family: serif">serif</span>

You can set font families like this:

```css
.my_class{
    font-family: cursive;
}
```

--- /collapse ---

--- collapse ---
---
title: Controlling text size
---

You can use the `font-size` properity to make your text look bigger, or smaller. The default size, which the user chooses and on which the others are based, is `medium`. The font sizes are:

  + <span style="font-size: xx-small">xx-small</span>
  + <span style="font-size: x-small">x-small</span>
  + <span style="font-size: small">small</span>
  + <span style="font-size: medium">medium</span>
  + <span style="font-size: large">large</span>
  + <span style="font-size: x-large">x-large</span>
  + <span style="font-size: xx-large">xx-large</span>
  + <span style="font-size: xxx-large">xxx-large</span>

You can set font sizes like this:

```css
.my_class{
    font-size: large;
}
```

--- /collapse ---

--- save --- 

**Test:** view `index.html` to see your text.


--- /task ---

--- task ---

Use a second class to give your paragraph a background colour. Once more, there are tips on doing this below.

--- collapse ---
---
title: Using more than one class for the same element
---

Sometimes it makes sense to use more than one class for the same element. You just separate the names of the classes with a space. You can use as many classes as you like this way. If the rules in two classes conflict, the rule that appears later in the CSS file will win.

```html
<div class="grid_tile red"> 
    <!-- some text/images/etc. in here --> 
</div>
```

A good example of when this is useful is when several elements are the same size and shape, but have different colours or fonts used on them.

--- /collapse ---

--- save --- 

**Test:** view `index.html` to see your new backgrounds.


--- /task ---

--- task ---

Include a video from YouTube in your grid (you can use [one of ours]((https://www.youtube.com/watch?v=knrrTxDYtdM)){:target="_blank"}, if you like).

--- collapse ---
---
title: Including YouTube video in your webpage
---

Including a video from YouTube on your webpage only takes a few steps: First, go to the video you want to include on YouTube and click the "share" button.

![The YouTube Share button](images/yt_share.png)

In the dialogue that opens you'll be shown a few ways you can share the video. Choose "Embed". Embedding means to include one thing inside another — this YouTube video will be embedded in your webpage.

![A number of buttons offering ways to share the video, including embed, WhatsApp, Facebook, Twitter, and Email.](images/yt_embed.png)

In the dialogue that opens you'll be shown a few options you can use to modfiy the version of the video that will be shared on your webpage. For now, just choose "Copy"

![The YouTube Share button](images/yt_share.png)

Paste the copied code into your webpage. This is an `iframe` tag. You don't need to understand exactly how it works just yet, but if you remove its `width` and `height` attributes then you can use your class for grid elements to apply the same settings to this video as you have used on `img` and `p` tags.
--- /collapse ---

--- save --- 

**Test:** view `index.html` to see your video.

--- /task ---

--- task ---

**Debug:** You might find some issues with your grid.

--- collapse ---
---
title: The container div doesn't appear
---

This is because the `float` property makes the `div`s in the grid behave a little differently, so they don't cause their container to grow. You can fix this by setting the `overflow` property on the container to `hidden`.

```css
.grid_container{
    background-color: green;
    margin-left: auto;
    margin-right: auto;
    overflow: hidden;
    width: 1200px;
}
```

--- /collapse ---

--- collapse ---
---
title: The divs in the grid start a new row without filling the current one completely
---

<div style="width: 180px; height: 120px; background-color: seagreen; margin: 10px auto;">
    <div style="width: 63px; height: 60px; background-color: skyblue;"> </div>
    <div style="width: 63px; height: 60px; background-color: skyblue;"> </div>
    <div style="width: 63px; height: 60px; background-color: skyblue;"> </div>
    <div style="width: 63px; height: 60px; background-color: skyblue;"> </div>
</div>

This is usually because the widths of the elements in the grid do not evenly add up to the width of the container. However, if you've also added a border to any of the `div`s in the grid, you need to work that into your maths too: If you have a two pixel border all the way around a `p`, you need to subtract four pixels (two for each side) from the width of the `p`.

--- /collapse ---

--- /task ---

