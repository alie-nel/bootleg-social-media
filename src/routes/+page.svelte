<script>
    import NavBar from "../components/navBar.svelte"
    import HomePage from "../components/home/homePage.svelte"
    import LoggedOutPage from "../components/home/loggedOutPage.svelte"
    import ExplorePage from "../components/explore/explorePage.svelte"

</script>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

<LoggedOutPage />

<NavBar />

<div class="home-page">

    <HomePage />
    <div class="explore-page">
        <ExplorePage />
    </div>
    
</div>

<style>
  :root {
        --dark-purple: #37186C;
        --medium-purple: #6742A6;
        --light-purple: #F3ECFF;
        --hover-purple: #78619E;
        --text-grey: #47464a;
        --hover-grey: #e9e8ea;
        --shadow-grey: #ebe7e7;
        --border-grey: #a7a8a4;
    }

    .home-page {
        display: flex;
        gap: 7vw;
        margin-left: 17vw;
    }

    @media (max-width: 750px) {
        .home-page {
            justify-content: center;
        }
    }

    @media (max-width: 750px) {
        .explore-page {
            display: none;
        }
    }

</style>