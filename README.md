#js
document.getElementById('login-form').addEventListener('submit', function(event) {
    event.preventDefault();
    // Perform validation or AJAX login request here
    // Example: For demonstration purposes, just alert the username
    const username = document.getElementById('username').value;
    alert(`Welcome, ${username}!`);
    // Redirect or perform further actions based on login success
});
#css
 {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}

.login-container {
    background-color: #fff;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 0 20px rgba(0, 0, 0, 0.1);
    width: 300px;
}

.login-form {
    display: flex;
    flex-direction: column;
}

.login-form h2 {
    text-align: center;
    margin-bottom: 20px;
}

.input-group {
    margin-bottom: 15px;
}

.input-group label {
    font-weight: bold;
    margin-bottom: 5px;
}

.input-group input {
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 4px;
    font-size: 16px;
}

.btn {
    background-color: #4CAF50;
    color: white;
    padding: 10px;
    border: none;
    cursor: pointer;
    border-radius: 4px;
    font-size: 16px;
}

.btn:hover {
    background-color: #45a049;
}

.register-link {
    text-align: center;
    margin-top: 10px;
}

.register-link a {
    color: #007bff;
    text-decoration: none;
}

.register-link a:hover {
    text-decoration: underline;
}
#html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fuel Finder - Login</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="login-container">
        <form id="login-form" class="login-form">
            <h2>Login to Fuel Finder</h2>
            <div class="input-group">
                <label for="username">Username</label>
                <input type="text" id="username" name="username" required>
            </div>
            <div class="input-group">
                <label for="password">Password</label>
                <input type="password" id="password" name="password" required>
            </div>
            <button type="submit" class="btn">Login</button>
            <p class="register-link">Don't have an account? <a href="#">Register here</a></p>
        </form>
    </div>

    <script src="script.js"></script>
</body>
</html>
