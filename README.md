# Flamed Lite
Flamed is currently in beta. This is an embedable version of it. 
*Flamed Lite might not have all games just like the main version.*
# HOW TO EMBED:
**Paste This HTML Code In A .html File**
```
<script>
  const fetchme = "https://cdn.jsdelivr.net/gh/Flamed-Games/Flamed-Lite@main/index.html";

  fetch(fetchme)
    .then(response => response.text())
    .then(html => {
      document.open();
      document.write(html);
      document.close();
    })
    .catch(err => {
      document.body.innerHTML = "<h1>Failed To Fetch Content | Powerd by Bloxcraft UBG</h1>";
      console.error(err);
    });
</script>

```
**NOTE: Check back once a week or month to see if we updated this, because this is in BETA too! This is the singlefile version that fetches with jsdeliver.**
