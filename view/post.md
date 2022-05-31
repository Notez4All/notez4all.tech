---
title: View an Upload!
---
<script src="https://cdn.jsdelivr.net/npm/ipfs/dist/index.min.js"></script>
<script>
var url = new URL(window.location.href);
var dId = url.searchParams.get("documentId");
console.log(dId);
var file = ipfs.get(dId);
document.getElementById('Doc').innerHtml("text");
</script>
<p id="text"></p>
