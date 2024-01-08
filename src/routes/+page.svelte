<script>
    import NavBar from "../components/navBar.svelte"
    import HomePage from "../components/home/homePage.svelte"
    import LoggedOutPage from "../components/home/loggedOutPage.svelte"
    import ExplorePage from "../components/explorePage.svelte"

    const loggedOut = false;

</script>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

<div class="home-page">
    {#if loggedOut}
        <LoggedOutPage />
    {/if}

    <HomePage />
    <ExplorePage/>
    <NavBar />
    
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
</style>