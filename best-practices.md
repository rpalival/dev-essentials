# Best Practices

---

## HTML

1. 99% of the time **use classes** instead of IDs coz there can only be 1 unique ID value
2. Always use **`<a>`** tag to have a link to go somewhere else
3. Know when to use div | article | section. [Difference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element#content_sectioning)
4. use class as a methodology for self-documentation purposes, label every tag with a class and use **descriptive** names
5. Optimize your code for the "forever" part of it and "writing" part of it

---

## CSS

---
1. **class selectors** in css can be used across different tag types but **tag selectors** will only work for same tags
2. Name the css **class names** based on **what they are** and not what they look like
3. Never use pseudo-classes such as :hover to implement core functionality because they do not work on mobile devices. Use them to add a little flair to web experience
4. Use this css code on every css file / project:<br>
This makes the element sizing of width include padding+border+content in it.
```css
    * {
        box-sizing: border-box;
    }
```
5. For better performance use:
```css
    html {
        box-sizing: border-box;
    }
    
    *, *::before, *::after {
        box-sizing: inherit;
    }

```
