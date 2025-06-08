<%*
const title = tp.file.title;
const parent = await tp.system.prompt("Nom du parent (facultatif)", "");
const related = await tp.system.prompt("Notes liées ? (séparées par virgule)", "");
const children = await tp.system.prompt("Notes enfants ? (séparées par virgule)", "");

const list = input => input ? input.split(",").map(i => "- " + i.trim()).join("\n") : "";
%>
---
tags: [juggl]
<% if (parent) { %>parent: <%= parent %><% } %>
<% if (related) { %>related:\n<%= list(related) %><% } %>
<% if (children) { %>children:\n<%= list(children) %><% } %>
---

# <%= title %>

> À compléter manuellement si besoin.

