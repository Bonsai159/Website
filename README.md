{
  margin: 0;
  padding: 0;
  font-family: "Poppins", sans-serif;
}

body {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  background: url('UU.jpg') no-repeat;
  background-size: cover;
  background-position: center;
}

header {
  position: fixed;
  top: 0;
  left: 0;
  width: 92%;
  padding: 20px 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  z-index: 99;
}

.logo{
  font-size: 2em;
  color: #000;
  user-select: none;
}

.navigation a {
  position: relative;
  font-size: 1.1em;
  color: #000;
  text-decoration: none;
  font-weight: 500;
  margin-left: 40px;
}

.navigation a::after {
  content: '';
  position: absolute;
  left: 0;
  bottom: -6px;
  width: 100%;
  height: 3px;
  background: #000;
  border-radius: 5px;
  transform-origin: right;
  transform: scaleX(0);
  transition: transform .5s;
}

.navigation a:hover::after {
  transform-origin: left;
  transform: scale(1);
}

.navigation .btnLogin-popup {
  width: 130px;  
  height: 50px;
  background: transparent;
  border: 2px solid #000;
  outline: none;
  border-radius: 6px;
  cursor: pointer;
  font-size: 1.1em;
  color: #000;
  font-weight: 500;
  margin-left: 40px;
  transition: .5s;
}

.navigation .btnLogin-popup:hover {
  background: skyblue;
  color: #162938;
}

.wrapper {
  position: relative;
  width: 400px;
  height: 440px;
  background: transparent;
  border: 2px solid rgba(255, 255, 255, .5);
  border-radius: 20px;
  backdrop-filter: blur(20px);
  box-shadow: 0 0 30px rgba(0, 0, 0, .5);
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden; 
  transform: scale(0);
  transition: transform .5s ease, height .2s ease;
}

.wrapper.active-popup {
  transform: scale(1);
  transition: transform .5s ease, height .2s ease;
}

.wrapper.active {
  height: 520px;
}

.wrapper .form-box {
  width: 100%;
  padding: 40px;
}

.wrapper .form-box.login{
  transition: transform .18s ease;
  transform: translateX(0);
}

.wrapper.active .form-box.login {
  transition: none;
  transform: translateX(-400px);
}

.wrapper .form-box.register {
  position: absolute;
  transition: none;
  transform: translateX(400px);
}

.wrapper.active .form-box.register {
  transition: transform .18s ease;
  transform: translateX(0);
}

.wrapper .icon-close {
  position: absolute;
  top: 0;
  right: 0;
  width: 45px;
  height: 45px;
  background: #162938;
  font-size: 2em;
  color: #fff;
  display: flex;
  justify-content: center;
  align-items: center;
  border-bottom-left-radius: 20px;
  cursor: pointer;
  z-index: 1;
}

.form-box h2 {
  font-size: 2em;
  color: #000;
  text-align: center;
}

.input-box {
  position: relative;
  width: 100%;
  height: 50px;
  border-bottom: 2px solid #000;
  margin: 30px 0;
}

.input-box label {
  position: absolute;
  top: 50%;
  left: 5px;
  transform: translateY(-50%);
  font-size: 1em;
  color: #000;
  font-weight: 500;
  pointer-events: none;
  transition: .5s;
}

.input-box input:focus~label,
.input-box input:valid~label {
  top: -5px;
}

.input-box input {
  width: 100%;
  height: 100%;
  background: transparent;
  border: none;
  outline: none;
  font-size: 1em;
  color: #000;
  font-weight: 600;
  padding: 0 35px 0 5px;
}

.input-box .icon {
  position: absolute;
  right: 8px;
  font-size: 1.2em;
  color: #000;
  line-height: 57px;
}

.remember-forgot {
  font-size: .9em;
  color: #000;
  font-weight: 500;
  margin: -15px 0 15px;
  display: flex;
  justify-content: space-between;
}

.remember-forgot label input {
  accent-color: #000;
  margin-right: 3px;
}

.remember-forgot a {
  color: #000;
  text-decoration: none;
}

.remember-forgot a:hover {
  text-decoration: underline;
}

.btn {
  width: 100%;
  height: 45px;
  background: #000;
  border: none;
  outline: none;
  border-radius: 6px;
  cursor: pointer;
  font-size: 1em;
  color: #fff;
  font-weight: 500;
}

.login-register {
  font-size: .9em;
  color: #000;
  text-align: center;
  font-weight: 500;
  margin: 25px 0 10px;
}

.login-register p a {
  color: #000;
  text-decoration: none;
  font-weight: 600;
}

.login-register p a:hover {
  text-decoration: underline;
}
