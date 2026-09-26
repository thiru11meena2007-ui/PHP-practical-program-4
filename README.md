# PHP-practical-program-4

<?php

session_start();

if ($_POST) {

if ($_POST["user"] == "admin" && $_POST["pass"] == "12345") {

$_SESSION["user"] = "admin";

echo "Login Successful!";

} else {

echo "Invalid Username or Password!";

}

}

?>

<!DOCTYPE html>

<html>

<head>

<title>Login</title>

</head>

<body>

<h2>Login Page</h2>

<form method="post">

Username: <input type="text" name="user"><br><br>

Password: <input type="password" name="pass"><br><br>

<input type="submit" value="Login">

</form>

</body>

</html>


Output
Login Page

Username: admin
Password: 12345

Login Successful!
