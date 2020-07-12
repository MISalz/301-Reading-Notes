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


### [home](https://misalz.github.io/reading_notes2/)