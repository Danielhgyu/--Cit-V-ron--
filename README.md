<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Пропускной пункт</title>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      background-color: #e74c3c;
      color: white;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      text-align: center;
      padding: 10px;
    }
    h2 {
      font-size: 2.5em;
      margin-bottom: 20px;
      color: #fff;
      text-transform: uppercase;
      letter-spacing: 3px;
    }
    .container {
      background: rgba(255, 255, 255, 0.1);
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
      width: 100%;
      max-width: 400px;
    }
    input {
      padding: 12px;
      font-size: 1.2em;
      width: 100%;
      border: 2px solid #fff;
      border-radius: 5px;
      background: transparent;
      color: white;
      text-align: center;
      margin-bottom: 20px;
    }
    button {
      padding: 12px 20px;
      font-size: 1.2em;
      background-color: #fff;
      color: #e74c3c;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: background-color 0.3s ease;
      width: 100%;
    }
    button:hover {
      background-color: #f39c12;
      color: white;
    }
    input:focus {
      outline: none;
      border-color: #f39c12;
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
    <button onclick="checkPassword()">Отправить</button>
  </div>
</body>
</html>

