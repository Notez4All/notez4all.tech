---
title: View an Upload!
---
<script>
var url_string = {{ page.url }}; //window.location.href
var url = new URL(url_string);
var c = url.searchParams.get("documentId");
console.log(c);
</script>
