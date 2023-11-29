<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Login Page</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }

    #login-container {
      text-align: center;
    }

    input {
      margin-bottom: 10px;
    }
  </style>
</head>
<body>

<div id="login-container">
  <h2>Login</h2>
  <form id="login-form">
    <label for="username">Username:</label>
    <input type="text" id="username" required>

    <label for="password">Password:</label>
    <input type="password" id="password" required>

    <button type="button" onclick="login()">Login</button>
  </form>

  <p id="error-message" style="color: red;"></p>
</div>

<script>
  function login() {
    const username = document.getElementById('username').value;
    const password = document.getElementById('password').value;

    // Perform simple client-side validation
    if (username === '' || password === '') {
      document.getElementById('error-message').textContent = 'Please enter both username and password.';
      return;
    }

    // Simulate server-side authentication
    // In a real-world scenario, you would send a request to a server for authentication
    // and handle the response accordingly.
    if (username === 'yourUsername' && password === 'yourPassword') {
      alert('Login successful! Redirecting to the dashboard...');
      // In a real-world scenario, you would redirect the user to the dashboard or another page.
    } else {
      document.getElementById('error-message').textContent = 'Invalid username or password.';
    }
  }
</script>

</body>
</html>
