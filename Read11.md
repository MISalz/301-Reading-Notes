# Read 11 Notes

# [EJS](https://www.youtube.com/playlist?list=PL7sCSgsRZ-slYARh3YJIqPGZqtGVqZRGt)


## Video2
app.set('views', path.join(_dirname,'views'));
app.set('view engine','ejs');

app.get('/', function(req,res){
    response.render('index');
})

** create a index.ejs file

## Video3

response.render takes in 3 params
* view string file name
* object local obj of variables
* local call back
### server.js
app.get('/', function(req,res){
    response.render('index{
        index : value,
    })
})
### index.ejs
/</div/><%= value %></div/>

## Video4

### server.js
app.get('/', function(req,res){
    response.render('index{
        people:[
        {name : 'dave'},
        ]
    })
})
### index.ejs
/</ul/>
<% for (let person of people){%>

<li><%=person.name %></li>
<% } %>
</ul/>

## Video5

if else statements

### index.ejs
/</ul/>
<% for (let person of people){%>
<% if (person.name ==='dave'){%>
<li><%=person.name %></li>
<% } %>
<% } %>

</ul/>

# Reading
https://ejs.co/#promo

## Options
cache Compiled functions are cached, requires filename<br>

filename Used by cache to key caches, and for includes<br>

root Set project root for includes with an absolute path (e.g, /file.ejs). Can be array to try to resolve include from multiple directories.<br>

views An array of paths to use when resolving includes with relative paths.<br>

context Function execution context<br>

compileDebug When false no debug instrumentation is compiled<br>

client Returns standalone compiled function<br>

delimiter<br>

openDelimiter<br>

closeDelimiter '/li><br>

debug Outputs generated function body<br>

strict When set to `true`, generated function is in strict mode<br>

_with Whether or not to use with() {} constructs. If false then the locals will be stored in the locals object. (Implies `--strict`)<br>

localsName Name to use for the object storing local variables when not using with Defaults to locals<br>

rmWhitespace Remove all safe-to-remove whitespace, including leading and trailing whitespace. It also enables a safer version of -%> line slurping for all scriptlet tags (it does not strip new lines of tags in the middle of a line).<br>

escape The escaping function used with <%= construct. It is used in rendering and is .toString()ed in the generation of client functions. (By default escapes XML).<br>

outputFunctionName Set to a string (e.g., 'echo' or 'print') for a function to print output inside scriptlet tags.<br>

async When true, EJS will use an async function for rendering. (Depends on async/await support in the JS runtime.<br>

# Tags
<% 'Scriptlet' tag, for control-flow, no output<br>
<%_ ‘Whitespace Slurping’ Scriptlet tag, strips all whitespace before it<br>
<%= Outputs the value into the template (HTML escaped)<br>
<%- Outputs the unescaped value into the template<br>
<%# Comment tag, no execution, no output<br>
<%% Outputs a literal '<%' <br>
%> Plain ending tag<br>
-%> Trim-mode ('newline slurp') tag, trims following newline<br>
_%> ‘Whitespace Slurping’ ending tag, removes all whitespace after it<br>

# Includes
Includes are relative to the template with the include call. (This requires the 'filename' option.) 

For example if you have "./views/users.ejs" and "./views/user/show.ejs" you would use <%- include('user/show'); %>.


### [home](https://misalz.github.io/reading_notes2/)