<script>
    import NavBar from "../components/navBar.svelte"
    import HomePage from "../components/home/homePage.svelte"
    import LoggedOutPage from "../components/home/loggedOutPage.svelte"
    import ExplorePage from "../components/explore/explorePage.svelte"

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

<div class="home-page">

    <NavBar />
    <HomePage />
    <ExplorePage />
    
</div>

<style>
  :root {
        --dark-purple: #37186C;
        --medium-purple: #6742A6;
        --shadow-grey: #ebe7e7;
    }

    .home-page {
        display: flex;
    }

    .login {
       display: flex;
       align-items: center;
       justify-content: center;
       position: absolute;
       width: 100vw;
       height: 100vh;
       z-index: 11;
  }

  .grey-cover {
        position: fixed;
        z-index: 10;
        top: 0;
        left: 0;
        width: 100vw;
        height: 100vh;
        background-color: grey;
        opacity: 0.2;
    }

    .login-box {
        position: relative;
        margin: auto;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        gap: 20px;
        padding: 40px 0 60px 0;
        z-index: 100;
        width: 400px;
        background-color: white;
        border-radius: 10px;
        box-shadow: 0 1.5px 1px #73736c;
        font-family: 'Roboto', sans-serif;
        box-sizing: border-box;
    }

    .login-title {
        margin: 0;
        font-size: 1.8rem;
    }

    .username {
        width: 300px;
        height: 30px;
        border-radius: 5px;
        border: 1px solid grey;
    }

    .password {
        width: 300px;
        height: 30px;
        border-radius: 5px;
        border: 1px solid grey;
    }

    .login-button {
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

    .hidden {
        display: none;
    }

</style>