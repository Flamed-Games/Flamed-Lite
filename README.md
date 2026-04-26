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

**If you want to embed this on a .svg file (NOT a image) here is the code:**

```
<svg xmlns="http://www.w3.org/2000/svg" width="100%" height="100%" style="position: fixed; top: 0; left: 0;">
  <foreignObject x="0" y="0" width="100%" height="100%">
    <body xmlns="http://www.w3.org/1999/xhtml">
      <meta content='width=device-width, initial-scale=1.0' name='viewport'></meta>
      <iframe style="position:fixed; top:0; left:0; bottom:0; right:0; width:100%; height:100%; border:none; margin:0; padding:0; overflow:hidden; z-index:999999;" id="game-frame"></iframe>
      
      <script>
  
        let code = "PHNjcmlwdD4KICBjb25zdCBmZXRjaG1lID0gImh0dHBzOi8vY2RuLmpzZGVsaXZyLm5ldC9naC9GbGFtZWQtR2FtZXMvRmxhbWVkLUxpdGVAbWFpbi9pbmRleC5odG1sIjsKCiAgZmV0Y2goZmV0Y2htZSkKICAgIC50aGVuKHJlc3BvbnNlID0+IHJlc3BvbnNlLnRleHQoKSkKICAgIC50aGVuKGh0bWwgPT4gewogICAgICBkb2N1bWVudC5vcGVuKCk7CiAgICAgIGRvY3VtZW50LndyaXRlKGh0bWwpOwogICAgICBkb2N1bWVudC5jbG9zZSgpOwogICAgfSkKICAgIC5jYXRjaChlcnIgPT4gewogICAgICBkb2N1bWVudC5ib2R5LmlubmVySFRNTCA9ICI8aDE+RmFpbGVkIFRvIEZldGNoIENvbnRlbnQgfCBQb3dlcmQgYnkgQmxveGNyYWZ0IFVCRzwvaDE+IjsKICAgICAgY29uc29sZS5lcnJvcihlcnIpOwogICAgfSk7Cjwvc2NyaXB0Pgo=";
        
        var theIframe = document.getElementById('game-frame');
        theIframe.srcdoc = atob(code);
      </script>
    </body>
  </foreignObject>
</svg>
```
