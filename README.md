# 
<!doctype html>
<html lang="en">
  <head>
    <title>Character Count Tool - Ichchha 23BIS70037</title>
    <style>
      body {
        font-family: Arial, sans-serif;
        margin: 40px;
      }
      textarea {
        width: 300px;
        height: 120px;
        font-size: 16px;
        padding: 10px;
        border: 2px solid #333;
        border-radius: 5px;
        resize: none;
      }
      p {
        font-size: 16px;
        margin-top: 10px;
        color: #333;
      }
    </style>
  </head>
  <body>
    <h3>Type your text:</h3>
  <textarea id="text" rows="5" cols="40" placeholder="Start Typing....."></textarea>
  <p>Characters: <span id="count">0</span></p>
  <script>
    const textarea = document.getElementById('text');
    const count = document.getElementById('count');

    textarea.addEventListener('input', function() {
      count.textContent = textarea.value.length;
    });
  </script>
  </body>
</html>
