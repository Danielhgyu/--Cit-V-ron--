<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Пропускной пункт</title>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      background-color: #282c34;
      color: white;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      text-align: center;
    }
    h2 {
      font-size: 3em;
      margin-bottom: 30px;
      color: #f39c12;
      text-transform: uppercase;
      letter-spacing: 3px;
    }
    .container {
      background: rgba(0, 0, 0, 0.7);
      padding: 40px;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
    }
    input {
      padding: 15px;
      font-size: 1.5em;
      width: 250px;
      border: 2px solid #f39c12;
      border-radius: 5px;
      background: transparent;
      color: white;
      text-align: center;
      margin-bottom: 20px;
    }
    button {
      padding: 15px 30px;
      font-size: 1.5em;
      background-color: #f39c12;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }
    button:hover {
      background-color: #e67e22;
    }
    input:focus {
      outline: none;
      border-color: #e67e22;
    }
  </style>
  <script>
    function checkPassword() {
      const password = document.getElementById('password').value;
      if (password === 'абсент') {
        window.location.href = 'https://example.com/доступ';
      } else {
        alert('Неверный пароль');
      }
    }
  </script>
</head>
<body>
  <div class="container">
    <h2>Введите пароль для доступа:</h2>
    <input type="password" id="password" placeholder="Пароль">
    <br>
    <button onclick="checkPassword()">Отправить</button>
  </div>
</body>
</html>

