<!DOCTYPE html>
<html>
<head>
<style>
body {
    font-family: Arial, sans-serif;
  background-image: url('C:/Users/Bahria/OneDrive/Pictures/Screenshots/Screenshot (129).PNG');
   background-repeat: no-repeat;

   
}
   #main{
         margin-top: 100px;
         font-family: verdana;
         font-size: 40px;
         color: white;
   }


/* Style the login container */
.login-container {
    width: 300px;
    padding: 16px;
    background-color: white;
    margin: 0 auto;
    margin-top: 100px;
    border: 1px solid black;
    border-radius: 4px;
}

/* Style the input fields */
.login-container input[type=text], .login-container input[type=password] {
    width: 90%;
    padding: 15px;
    margin: 5px 0 22px 0;
    border: none;
    background: #f1f1f1;
}

/* Style the remember me checkbox */
.login-container input[type=checkbox] {
    margin-bottom: 15px;
}

/* Style the submit button */
.login-container .btn {
    background-color: #4CAF50;
    color: white;
    padding: 14px 20px;
    margin: 8px 0;
    border: none;
    cursor: pointer;
    width: 100%;
    opacity: 0.9;
}

.login-container .btn:hover {
    opacity:1;
}

/* Style the links to other pages */
.login-container a {
    color: black;
    text-decoration: none;
}

.login-container a:hover {
    text-decoration: underline;
}
</style>
</head>
<body>

   <center><h1 id="main">Login Form</h1></center>

<div class="login-container">
    <form action="/login" method="post">
        <label for="email"><b>Email</b></label>
        <input type="text" placeholder="Enter Email" name="email" required>

        <label for="psw"><b>Password</b></label>
        <input type="password" placeholder="Enter Password" name="psw" required>

        <label for="remember">
            <input type="checkbox" name="remember" id="remember"> Remember me
        </label>

        <button type="submit" class="btn">Login</button>
    </form>

    <div style="margin-top: 20px;">
        <a href="/forgot-password">Forgot password?</a> 
        
        <br/>
        <p>Don't have an account? <a href="/register">Register</a></p>
       
</div>

</body>
</html>
