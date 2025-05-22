<!DOCTYPE html>
<html>
<head>
  <title>Zawad's Request</title>
</head>
<body>
  <h1>Hi,World!</h1>
  <p>I'm Zawad. Nice to meet you all!</p>
  <p>I want to say something to everyone.<br>Can any of you lend me 20tk?? pls 🙏 🥺 </p>

  <button onclick="openInChrome()">Yes</button>
  <button onclick="openInChrome()">Obviously</button>
  <button onclick="openInChrome()">I will give you 100tk, love😘</button>

  <script>
    function openInChrome() {
      // Tries to open in Chrome on Android, else opens in default browser
      const url = "https://postimg.cc/7fP7zWb5";
      const chromeScheme = "googlechrome://navigate?url=" + url;

      // For Android Chrome
      if (navigator.userAgent.includes("Android")) {
        window.location.href = chromeScheme;
        setTimeout(() => {
          window.location.href = url;
        }, 500);
      } else {
        // For desktop and others
        window.open(url, '_blank');
      }
    }
  </script>
</body>
</html>
