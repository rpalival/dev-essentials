
### Key Terminologies

---

| Term | Definition | Meaning |
| ---- | --------------------- | ------ |
| HTML | Hyper Text Markup Language |
| HTML Tags | shows what Type of content is inside the tag (semantic meaning) |
| Opening Tag | `< >` |
| Closing Tag | `</ >` |
| Self Closing Tag /<br> Void Tags | `< />` |
| Attribute | key = "value"| what kind of tag it is and every tag has suitable list of attributes 
| Class | class = "value" <br> class = "value1 value2 value3"| the value is the styling part and will get implemented for the tag on which this class is used


#### Common Tags

---

> Tags have default margins based on browser, Be Aware when handling CSS!

| Term | Syntax | Definition
| ---- | --------------------- | --------
| Header Tags | `<h1> </h1>...<h6> </h6>` | Main Heading with 5 levels of sub heading
| Paragraph Tag | `<p> </p>` | Group text and create space
| Anchor Tag | `<a href="destination-url"> display-text</a>` | Create links that takes to destination webpage
| Division Tag| `<div> </div>` | A box or generic container
| Span Tag| `<span> </span>`| A ziplock bag or generic container for small pieces of text
| ordered list Tag| `<ol>`<br>&nbsp;&nbsp;&nbsp;&nbsp;`<li> item </li>`<br>`</ol>` | Numbers each item from 1...n in a list
| unordered list Tag| `<ul>`<br>&nbsp;&nbsp;&nbsp;&nbsp;`<li> item </li>`<br>`</ul>` | Bullet points each item from 1...n in a list
|list item Tag| `<li>item</li>`| creating individual items in a list
|Button Tag| `<button>button-name</button>`| Creates clickable button
|Image Tag| `<img src=" " alt=" " />`| if its background image use CSS otherwise use img tag
|Input Tag| `<input />`| To gather user input, lot of [types](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input#input_types) available and [attributes](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input#attributes) <br> 
|Text Area Tag| `<textarea> </textarea>`| Expandable Text input area
|Select and Option| `<select>`<br>&nbsp;&nbsp;&nbsp;`<option value=""> item </option>`<br>`</select>`| It's like a dropdown button with list of options to choose value from (not sure if we can choose multiple values)
|Form Tag| `<form></form>`| A group of html tags related to gathering data from a user, it may include input, textarea, and many other tags.
|Table Tag| `<table> </table>`| It creates a table with rows and columns along with caption and footer row <br> 1. `<caption></caption>`: Table Title <br> 2. `<thead></thead>`: Column header row <br> 3. `<tbody> </tbody>`: Table body <br> 4. `<tr></tr>`: Table row <br> 5. `<th scope="row"/"col"> </th>`: Header cell <br> 6. `<td> </td>`: Data cell <br> 7. `<tfoot> </tfoot>`: last row showing column summary
| Navigation Tag | `<nav></nav>`| A common block from where user can find the links of all the places they can visit on/from my webpage.

---

#### Common Attributes

---

| Attribute | Syntax | Common values |
| ---- | --------------------- | ------ |
| href| `<a href="">` | url link of where you wanna go <br> it can be relative link or absolute link