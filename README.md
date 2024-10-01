<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width">
  <title>replit</title>
  <link href="style.css" rel="stylesheet" type="text/css" />
</head>

<body>
  
  <header>
    <h2 class="logo">Study Thing</h2>
    <nav class="navigation">
      <a href="#">Home</a>
      <a href="#">About</a>
      <a href="#">Services</a>
      <a href="#">Contact</a>
      <button class="btnLogin-popup">Login</button>
    </nav>
  </header>

  <div class="wrapper">
    <span class="icon-close"><ion-icon name="close-outline"></ion-icon>
    </span>
    
    <div class="form-box login">
      <h2>Login</h2>
      <form action="#">
        <div class="input-box">
          <span class="icon"><ion-icon name="mail"></ion-icon>
          </span>
          <input type="email" required>
          <label>Email</label>
        </div>
        <div class="input-box">
          <span class="icon"><ion-icon name="lock-closed"></ion-icon></span>
          <input type="password" required>
          <label>Password</label>     
        </div>
        <div class="remember-forgot">
          <label><input type="checkbox">Remember me</label>
          <a href="#">Forgot Password?</a>
        </div>
        <button type="submit" class="btn">Login</button>
        <div class="login-register">
          <p>Don't have an account?<a href="#"
          class="register-link">Register</a></p>
        </div>
      </form>  
    </div>    

    <div class="form-box register">
      <h2>Registration</h2>
      <form action="#">
        <div class="input-box">
          <span class="icon"><ion-icon name="person"></ion-icon>
          </span>
          <input type="text" required>
          <label>Username</label>
        </div>
        <div class="input-box">
          <span class="icon"><ion-icon name="mail"></ion-icon>
          </span>
          <input type="email" required>
          <label>Email</label>
        </div>
        <div class="input-box">
          <span class="icon"><ion-icon name="lock-closed"></ion-icon></span>
          <input type="password" required>
          <label>Password</label>     
        </div>
        <div class="remember-forgot">
          <label><input type="checkbox">I agree to the terms & conditions</label>
        </div>
        <button type="submit" class="btn">Register</button>
        <div class="login-register">
          <p>Already have an account?<a href="#"
          class="login-link">Login</a></p>
        </div>
      </form>  
    </div>    
  </div>    

  
  <script src="script.js"></script>
  <script type="module" src="https://unpkg.com/ionicons@7.1.0/dist/ionicons/ionicons.esm.js"></script>
  <script nomodule src="https://unpkg.com/ionicons@7.1.0/dist/ionicons/ionicons.js"></script>  
</body>

</html>

