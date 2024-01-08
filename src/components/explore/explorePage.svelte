<script>
    import SearchBar from "./searchBar.svelte";
    import TrendingPage from "./trendingPage.svelte";
</script>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

    <div class="explore">

        <h1 class="search-title">Search</h1>
        <SearchBar />

        <h1 class="trending-title">Trending</h1>
        <TrendingPage />

    </div>

<style>
    .explore {
        margin-left: 200px;
        width: 350px;
        font-family: 'Roboto', sans serif;
    }

    .search-title {
        font-size: 1.5rem;
        color: #37186C;
    }

    .trending-title {
        font-size: 1.5rem;
        color: #37186C;
    }

</style>