# Flamed Lite
Flamed is currently in beta. This is an embedable version of it. 
*Flamed Lite might not have all games just like the main version.*
# HOW TO EMBED:
**Paste This HTML Code In A .html File**
```
<script>
    launch();

    function launch() {
      try {
        fetch("https://cdn.jsdelivr.net/gh/Flamed-Games/Flamed-Lite@main/flamed.html?t="+Date.now())
          .then(response => response.text())
          .then(html => {
                document.documentElement.innerHTML = html;

                document.documentElement.querySelectorAll('script').forEach(oldScript => {
                    const newScript = document.createElement('script');
                    if (oldScript.src) {
                        newScript.src = oldScript.src;
                    } else {
                        newScript.textContent = oldScript.textContent;
                    }
                    document.body.appendChild(newScript);
                });
          });
      } catch (error) {
        console.error('error:', error);
      }
    }
  </script>
```
