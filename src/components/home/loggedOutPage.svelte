<script>
    
</script>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

<section class="login-page">

    <div class="grey-cover">

    </div>

    <section class="login">
        <h3 class="login-title">LOGIN</h3>
        <input class="username" type="input" placeholder="Username or email">
            <input class="password" type="password" placeholder="Password">
        <button class="login-button" type="submit">LOGIN</button>

    </section>

</section>


<style>

  .login-page {
       position: fixed;
  }

  .grey-cover {
        position: fixed;
        z-index: 10;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: grey;
        opacity: 0.2;
    }

    .login {
        position: absolute;
        z-index: 10;
        margin-top: 70px;
        margin-left: 430px;
        width: 400px;
        height: 380px;
        background-color: white;
        border-radius: 10px;
        box-shadow: 0 1.5px 1px #73736c;
        font-family: 'Roboto', sans-serif;
    }

    .login-title {
        margin-top: 40px;
        margin-bottom: 20px;
        margin-left: 153px;
        font-size: 30px;
    }

    .username {
        margin-top: 20px;
        margin-bottom: 10px;
        margin-left: 45px;
        width: 300px;
        height: 30px;
        border-radius: 5px;
        border: 1px solid grey;
    }

    .password {
        margin-top: 20px;
        margin-bottom: 10px;
        margin-left: 45px;
        width: 300px;
        height: 30px;
        border-radius: 5px;
        border: 1px solid grey;
    }

    .login-button {
        margin-top: 20px;
        margin-left: 157px;
        width: 80px;
        height: 35px;
        border: none;
        border-radius: 5px;
        background-color: #37186C;
        color: white;
        box-shadow: 0 2px 1px #ebe7e7;
        transition: background-color 0.2s;
    }

    .login-button:hover {
        cursor: pointer;
        color: #6742A6;
        background-color: #F3ECFF;
    }

</style>