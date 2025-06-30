<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <link rel="stylesheet" href="yy.css">
  <title>9TS</title>
</head>
<body>

  <video class="bg-video" autoplay muted loop playsinline>
    <source src="zz.mp4" type="video/mp4">
  </video>

  <div class="overlay">
    <h1>ℕ𝕚𝕜𝕜𝕜 𝕁𝕖𝕕𝕖𝕥𝕖𝕜𝕜𝕜𝕜𝕜𝕜𝕜𝕜𝕜𝕜𝕜𝕜</h1>
    <H3>𝕋𝕒𝕨 𝕥𝕒𝟝𝕣𝕒𝕝𝕚𝕚𝕚𝕚𝕚𝕚𝕚𝕚𝕚𝕚𝕚𝕚 𝕗𝕚𝕙</H3>
    <div id="ip">Getting your IP...</div>
    <br>
    <br>    <br>
    <br>    <br>
    <br>    <br>
    <br>    <br>
    <br>    <br>
    <br>    <br>
    <br>
  </div>

  <script>
fetch('https://api.ipify.org?format=json')
  .then(response => response.json())
  .then(data => {
    const ipElement = document.getElementById('ip');
    ipElement.textContent = `Your IP: ${data.ip}`;

    ipElement.style.fontSize = "24px"; 
    ipElement.style.color =  "#800000" ;
    ipElement.style.fontFamily = "Courier New" ;
  })
  .catch(() => {
    document.getElementById('ip').textContent = "Failed to get IP.";
  });

  </script>

</body>
</html>
