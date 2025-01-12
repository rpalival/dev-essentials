
### Key Terminologies

---

| Term                             | Definition                                                       | Meaning                                                                                             |
| -------------------------------- | ---------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| HTML                             | Hyper Text Markup Language                                       |
| HTML Tags                        | shows what Type of content is inside the tag (semantic meaning)  |
| Opening Tag                      | `< >`                                                            |
| Closing Tag                      | `</ >`                                                           |
| Self Closing Tag /<br> Void Tags | `< />`                                                           |
| Attribute                        | key = "value"                                                    | what kind of tag it is and every tag has suitable list of attributes                                |
| Class                            | class = "value" <br> class = "value1 value2 value3"              | the value is the styling part and will get implemented for the tag on which this class is used      |
| CSS Rule                         | selector tag {<br>&nbsp;&nbsp;&nbsp;&nbsp;property: value;<br> } | The tag is called selector<br>the styles defined in the rule will get applied to every matching tag |
| Parent & children Tags           |                                                                  | The css properties of parent will be applied to its children (Not all properties though)            |
| CSS Rule                         | .class<br> {<br>&nbsp;property: value;<br>}                      | the dot searches for class name as selector                                                         |
|||



#### Common Tags

---

> Tags have default margins based on browser, Be Aware when handling CSS!

| Term               | Syntax                                                                            | Definition                                                                                                                                                                                                                                                                                                                                                                               |
| ------------------ | --------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Header Tags        | `<h1> </h1>...<h6> </h6>`                                                         | Main Heading with 5 levels of sub heading                                                                                                                                                                                                                                                                                                                                                |
| Paragraph Tag      | `<p> </p>`                                                                        | Group text and create space                                                                                                                                                                                                                                                                                                                                                              |
| Anchor Tag         | `<a href="destination-url"> display-text</a>`                                     | Create links that takes to destination webpage                                                                                                                                                                                                                                                                                                                                           |
| Division Tag       | `<div> </div>`                                                                    | A box or generic container                                                                                                                                                                                                                                                                                                                                                               |
| Span Tag           | `<span> </span>`                                                                  | A ziplock bag or generic container for small pieces of text                                                                                                                                                                                                                                                                                                                              |
| ordered list Tag   | `<ol>`<br>&nbsp;&nbsp;&nbsp;&nbsp;`<li> item </li>`<br>`</ol>`                    | Numbers each item from 1...n in a list                                                                                                                                                                                                                                                                                                                                                   |
| unordered list Tag | `<ul>`<br>&nbsp;&nbsp;&nbsp;&nbsp;`<li> item </li>`<br>`</ul>`                    | Bullet points each item from 1...n in a list                                                                                                                                                                                                                                                                                                                                             |
| list item Tag      | `<li>item</li>`                                                                   | creating individual items in a list                                                                                                                                                                                                                                                                                                                                                      |
| Button Tag         | `<button>button-name</button>`                                                    | Creates clickable button                                                                                                                                                                                                                                                                                                                                                                 |
| Image Tag          | `<img src=" " alt=" " />`                                                         | if its background image use CSS otherwise use img tag                                                                                                                                                                                                                                                                                                                                    |
| Input Tag          | `<input />`                                                                       | To gather user input, lot of [types](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input#input_types) available and [attributes](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input#attributes) <br>                                                                                                                                                            |
| Text Area Tag      | `<textarea> </textarea>`                                                          | Expandable Text input area                                                                                                                                                                                                                                                                                                                                                               |
| Select and Option  | `<select>`<br>&nbsp;&nbsp;&nbsp;`<option value=""> item </option>`<br>`</select>` | It's like a dropdown button with list of options to choose value from (not sure if we can choose multiple values)                                                                                                                                                                                                                                                                        |
| Form Tag           | `<form></form>`                                                                   | A group of html tags related to gathering data from a user, it may include input, textarea, and many other tags.                                                                                                                                                                                                                                                                         |
| Table Tag          | `<table> </table>`                                                                | It creates a table with rows and columns along with caption and footer row <br> 1. `<caption></caption>`: Table Title <br> 2. `<thead></thead>`: Column header row <br> 3. `<tbody> </tbody>`: Table body <br> 4. `<tr></tr>`: Table row <br> 5. `<th scope="row"/"col"> </th>`: Header cell <br> 6. `<td> </td>`: Data cell <br> 7. `<tfoot> </tfoot>`: last row showing column summary |
| Navigation Tag     | `<nav></nav>`                                                                     | A common block from where user can find the links of all the places they can visit on/from my webpage.                                                                                                                                                                                                                                                                                   |

---

#### Common Attributes

---

| Attribute | Syntax        | Common values                                                                |
| --------- | ------------- | ---------------------------------------------------------------------------- |
| href      | `<a href="">` | url link of where you wanna go <br> it can be relative link or absolute link |

---

#### CSS Properties

---

| Property        | example              | Meaning                                                          |
| --------------- | -------------------- | ---------------------------------------------------------------- |
| color           | color: red;          | font color                                                       |
| font-size       | font-size: 60px;     |
| font-weight     | font-weight: normal; | How thin/thick the font is                                       |
| text-decoration | underline;           | underlines the text                                              |
| border          | 3px solid pink;      | creates a border around the tag of specified thickness and color |
| text-transform  | uppercase;           | text to uppercase                                                |
| border-radius   | 25px;                | makes the border corners rounded                                 |
| list-style      | upper-roman;         | instead of just round dots you can use these                     |
---

#### CSS Cascading Rules

___

> Some key points about CSS cascade rules:
> When specificity is equal, the last rule defined wins
> Direct styles override inherited styles
> Multiple classes are cumulative (e.g., .box.red has specificity of 20)
> Combining selectors adds their values (e.g., div#header has 101)

| Priority | Selector Type                | Example                        | Specificity Value |
| -------- | ---------------------------- | ------------------------------ | ----------------- |
| 1        | !important                   | color: red !important;         | Trumps all        |
| 2        | Inline styles                | <div style="color: red">       | 1000              |
| 3        | ID selectors                 | #header                        | 100               |
| 4        | Class/Attribute/Pseudo-class | .active, [type="text"], :hover | 10                |
| 5        | Elements/Pseudo-elements     | div, p, ::before               | 1                 |
| 6        | Universal selector           | *                              | 0                 |
| 7        | Inherited styles             | inherited from parent          | Lowest            |

---

#### CSS Pseudo-Classes

---

| pseudo-class| what it does?
| ---- | ----
|:hover| something happens when you hover over the element
|:first-child| something happens to the first element in a list
|:last-child| something happens to the last element in a list
|:nth-child(n)| something happens to the nth element in a list
|||