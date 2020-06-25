# Read 3 Notes

# [Mustache](https://medium.com/@1sherlynn/javascript-templating-language-and-engine-mustache-js-with-node-and-express-f4c2530e73b2)

Mustache is a logic-less template syntax. It can be used for HTML, config files, source code — anything. It works by expanding tags in a template using values provided in a hash or object.
It is often referred to as “logic-less” because there are no if statements, else clauses, or for loops. Instead, there are only tags. Some tags are replaced with a value, some nothing, and others a series of values.

Mustache.render/(“Hello, {{name}}”, { name: “Sherlynn” });
// returns: Hello, Sherlynn

two braces around {{ name }}. This is Mustache syntax to show that it is a placeholder

Then in the router configuration, use res.render(TEMPLATE_NAME, JSON_DATA). Example:
res.render('hello', {"name": "Sherlynn"})
Whereby the first parameter ‘hello’ refers to the hello.html file (no need to include the extension (e.g. hello.html) as it has been previously set as html.
The second parameter would be the JSON data itself. We can also pass in a variable representing the data, for example:
var nameObject = {"name": "Sherlynn"}
res.render('hello', nameObject)

# [flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

aims at providing a more efficient way to lay out, align and distribute space among items in a container, even when their size is unknown and/or dynamic (thus the word “flex”).

<img src="./images/read03 -img1.gif">

# [FlexboxFroggy](https://flexboxfroggy.com/)

Flexbox practice

<img src="./images/read03-img2.gif">

### [home](https://misalz.github.io/reading_notes2/)