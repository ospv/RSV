# RSV
Store analysis performed in the context of RSV mass vaccination in the US

<html>
  <body>
    <script>
      (async () => {
        const response = await fetch('https://api.github.com/repos/:user/:repo/contents/');
        const data = await response.json();
        let htmlString = '<ul>';
        
        for (let file of data) {
          htmlString += `<li><a href="${file.path}">${file.name}</a></li>`;
        }

        htmlString += '</ul>';
        document.getElementsByTagName('body')[0].innerHTML = htmlString;
      })()
    </script>
  <body>
</html>
