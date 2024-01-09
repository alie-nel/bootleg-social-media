<script>
    
    let hidden = false;
    
    const logIn = () => {
        hidden = !hidden;
    }
</script>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

<div class:hidden>

    <div class="grey-cover">
    </div>

    <section class="login">

        <form class="login-box">
            <h3 class="login-title">LOGIN</h3>
            <input class="username" type="input" placeholder="Username or email" required>
                <input class="password" type="password" placeholder="Password" required>
            <button class="login-button" type="submit" on:click={logIn}>LOGIN</button>

        </form>

    </section>

</div>

<style>

  

</style>