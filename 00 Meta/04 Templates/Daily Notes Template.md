---
<%*
const title = tp.file.title;
const yesterday = moment(title).subtract(1, 'days').format("YYYY-MM-DD");
const today = moment(title).format("YYYY-MM-DD");
const tomorrow = moment(title).add(1, 'days').format("YYYY-MM-DD");
-%>
cssclass: dailynote
fc-category: DNP
fc-calendar: Unified
fc-date: <% today %>
---
# [[<% yesterday %>|←]] <% today %> [[<% tomorrow %>|→]]

## Minor Tasking

## Gratitude 

## Health

## Accomplishments

```query
[[<% tp.file.title %>]] -path:Readwise -path:Dated
```

## Media Log 

```query
Imported: [[<% today %>]]
```