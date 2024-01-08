<script>
    import NewPost from "../newPost.svelte"
    import FeedComponent from "./feedComponent.svelte"
</script>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

<section class="home-section">

    <h1 class="home-title">Home Page</h1>
    <NewPost />

    <FeedComponent />
    
</section>

<style>
    .home-section {
        margin-left: 105px;
        min-width: 350px;
        width: 40vw;
        font-family: 'Roboto', sans-serif;
    }

    .home-title {
        color: var(--dark-purple);
    }

    .home-title:hover {
        cursor: default;
    }

</style>