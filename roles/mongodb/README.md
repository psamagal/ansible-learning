# <%= name %>

<%= description %>

## Usage

```sh
$ git submodule add <URL> roles/<%= name %>
```

<% if (typeof dependencies == "array") { %>
## Dependencies
<% for(var i = 0; i < dependencies.length; i++) { %>
- <%= dependencies[i] %>
<% } %>
<% } %>

Author: <% if (typeof author != "undefined") { %><%= author %><% } %> <% if (typeof email != "undefined") { %>(<%= email %>)
<% } %>