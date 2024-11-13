<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Facebook Ad Form</title>
<style>
  body {
    font-family: Arial, sans-serif;
    background-color: #f5f5f5;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }

  .form-container {
    background-color: #ffffff;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    padding: 20px;
    width: 300px;
  }

  .form-container label {
    font-weight: bold;
    color: #333333;
    display: block;
    margin-bottom: 8px;
  }

  .form-container input[type="text"],
  .form-container input[type="email"],
  .form-container input[type="tel"] {
    width: 100%;
    padding: 10px;
    margin-bottom: 15px;
    border: 1px solid #cccccc;
    border-radius: 4px;
    box-sizing: border-box;
  }

  .form-container input[type="submit"] {
    width: 100%;
    padding: 10px;
    background-color: #4267B2; /* Facebook blue */
    color: #ffffff;
    border: none;
    border-radius: 4px;
    font-weight: bold;
    cursor: pointer;
    transition: background-color 0.3s;
  }

  .form-container input[type="submit"]:hover {
    background-color: #365899;
  }
</style>
</head>
<body>

<div class="form-container">
  <form action="YOUR_SERVER_POST_URL" method="POST">
    <label for="name">Name</label>
    <input type="text" id="name" name="name" maxlength="40" required>

    <label for="phone">Phone Number</label>
    <input type="tel" id="phone" name="phone" maxlength="15" required>

    <label for="email">Email ID</label>
    <input type="email" id="email" name="email" maxlength="80" required>

    <input type="submit" value="Submit">
  </form>
</div>

</body>
</html>
