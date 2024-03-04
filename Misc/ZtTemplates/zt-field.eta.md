[title: "<%= it.title %>"
citekey: "<%= it.citekey %>"](<cssclasses: [%3C% null %%3E] 
aliases: [<% null %>]
type: <%= it.type %>
authors: [<%= it.authors %>]
title: "<%= it.title %>"
publication: <%= it.publicationTitle %>
date: <%= it.date %>
archive: <%= it.archive %>
archive-location: <%= it.archiveLocation %>
abstract: "<%= it.abstractNote %>"
citekey: "<%= it.citekey %>"
created: <%= it.dateAdded %>
modified: <%= it.dateModified %>
collections: <% for (const $it of it.collections) { %>
  <%= $it %>
<% } %>
people: [<% null %>]
themes: [<% null %>]
chapters: [<% null %>]
timeline: [<% null %>]
tags: <% it.tags.forEach(($it, i) => { %>
  <%= $it %>
<% }) %>
status: [<% null %>]>)