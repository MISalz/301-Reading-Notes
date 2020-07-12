# Read 12 Notes

## Video7

## partials

use parts of another file 
UseCase - Navbar, Footer
<%- include ('partials/onepartial) %>

## [Reading](https://medium.com/@henslejoseph/ejs-partials-f6f102cb7433)

Partials come in handy when you want to reuse the same HTML across multiple views. Think of partials as functions, they make large websites easier to maintain as you don’t have to go and change a piece of text in every page it appears in. 

In EJS, any JavaScript or non-HTML syntax you include in your templates is always surrounded by <% %> delimiters (you could change these delimiters if you really wanted to).

Including a partial in EJS is quite straightforward. You use <%- include( PARTIAL_FILE ) %> where the partial file is relative to the template you use it in.

**Note:** The <%- %> tags allow us to output the unescaped content onto the page (notice the -). This is important when using the include() statement since you don’t want EJS to escape your HTML characters like ‘<’, ‘>’,

### [home](https://misalz.github.io/reading_notes2/)