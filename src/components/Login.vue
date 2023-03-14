<template>
 <div class="container">
        <form action="">
            <div class="logo">

                <img class="imagelogo"  src="../assets/cloudnuro logo.png" alt="CloudNuro Logo">
            </div>
            <div class="form-group">
                <label for="">Email address</label>
                <input type="email" class="form-control" required>

            </div>
            <div class="form-group">
                <label for="">Password</label>
                <input type="password" class="form-control" required>

            </div>
            <input type="submit" class="btn" value="Sign In">
            <div class="forgot">
                <a href="#forgot">Forgot password ?</a>
            </div>
                <div class="line"></div>
                <div >
                    <p class="signin" >
                        <a href="#signin">Sign In </a>using custom domain ?
                    </p>
                </div>
        </form>
    </div>
</template>

<script>
export default {
  name: 'Login',
  
}
</script>

<style>
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body{
    min-height: 100vh;
    background-color:  #f8f7f7;;
    font-family: sans-serif;
}
.container{

    width: 100%;
    height: 100vh;
    position: relative;

}

.container form{
    width: 435px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
    padding: 50px;
    background-color: white;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(158,201,250,.3);;
}
.container form .imagelogo{

    display: block;
      margin: 0 auto;
      max-width: 180px;
      margin-bottom: 20px;
}
.container form .form-control{
    width :100%;
    height: 40px;
    border-radius: 4px;
    border: 1px solid silver;
    margin: 10px 0 18px 0;
    padding: 0 10px;
}
.container form .btn{
    width: 100%;
    height: 34px;
    background: #8f23e7;
    outline: none;
    border: none;
    font-size: 16px;
    color: white;
    cursor: pointer;
    border-radius: 4px;
    transition: .3s;
    padding: 8px 16px;
}
.container form .signin{
      text-align: center;
      font-size: small;
    padding: 12px 0;

}
.container form .forgot{
      text-align: center;
      font-size: small;
    padding: 12px 0;

}
a{
    text-decoration: none;
}
.form-group label{
    font-size: 14px;
}
.container form .line{
   
    border: 0;
    height: 1px;
    background: rgb(165, 160, 160);  
    margin: auto;
    width: 70%;

}
.container form .btn:hover{
    opacity: .9;
}




@media (max-width: 501px) {
  html {
    font-size: 15px;
  }

  .container form {
    width: 300px;
  }
}
</style>