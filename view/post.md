---
title: View an Upload!
---
<script src="https://cdn.jsdelivr.net/npm/ipfs/dist/index.min.js"></script>
<script>
var url = new URL(window.location.href);
var dId = url.searchParams.get("documentId");
console.log(dId);
for await (const buf of Ipfs.get(cid)) {
  document.getElementById("text").innerText(buf);
}
</script>
<p id="text"></p>
