
--- question ---

---
legend: Question 3 of 3
---

With the CSS and HTML provided below, what will the paragraph of text look like?

```html
<p class="core_paragraph light_background">The text will look like this.<p>
```

```css
body{
  color: black;
  background-color: gold;
}

.core_paragraph{
  color: green;
  background-color: blue;
}

.light_background{
  background-color: pink;
}
```

--- choices ---

- ( ) <span style="color: black; background-color: gold;">The text will look like this.</span>


  --- feedback ---
  This is what the text would look like if the paragraph didn't have any classes, and was just getting its rules from being inside the `body` tag.
  --- /feedback ---

- ( ) <span style="color: green; background-color: blue;">The text will look like this.</span>


  --- feedback ---
  This is what the text would look like if it only had the `core_paragraph` class in the CSS but it also has `light_background`. It would also look like this if `core_paragraph` appeared after `light_background` in the CSS file.
  --- /feedback ---

- ( ) <span style="color: black; background-color: pink;">The text will look like this.</span>


  --- feedback ---
  This is what the text would look like if it only had the `light_background` class, but it also has `core_paragraph`.
  --- /feedback ---

- (x) <span style="color: greem; background-color: pink;">The text will look like this.</span>


  --- feedback ---
  Correct! The `core_paragraph` class will give it green text, but the rule giving it a blue background will be replaced by the rule in `light_background` that sets the background to pink.
  --- /feedback ---

--- /choices ---

--- /question ---
