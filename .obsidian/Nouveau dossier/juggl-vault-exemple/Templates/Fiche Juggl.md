<%*
const title = tp.file.title; 
const parent = await tp.system.prompt("Nom du parent (optionnel)", ""); 
const related = await tp.system.prompt("Notes liées (séparées par virgule)", "");
const children = await tp.system.prompt("Enfants (séparés par virgule)", ""); 
const formatList = input => input.split(",").map(e => "  - " + e.trim()).join("\n");
%>
---
tags: [juggl]
<% if (parent) { %>parent: <%= parent %><% } %>
<% if (related) { %>related:
<%= formatList(related) %><% } %>
<% if (children) { %>children:
<%= formatList(children) %><% } %>
---

# <%= title %>

> Description rapide à compléter ici.
