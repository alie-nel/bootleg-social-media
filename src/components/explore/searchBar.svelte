<script>

</script>

  <div class="search">
    <input type="search" class="search-bar" placeholder="What are you looking for?">
    <button class="search-button"><i class="fa fa-search"></i></button>
  </div>

<style>
  .search {
        display: flex;
    }
    
    .search-bar {
        width: 260px;
        height: 45px;
        margin-bottom: 50px;
        font-size: 0.9rem;
        border: 1.2px solid var(--border-grey);
        border-radius: 5px;
        box-shadow: 0 2px 1px var(--shadow-grey);
    }
    .search-button {
        margin-left: 5px;
        width: 45px;
        height: 45px;
        border: none;
        border-radius: 5px;
        box-shadow: 0 2px 1px var(--shadow-grey);
        background-color: var(--dark-purple);
        color: white;
        transition: background-color 0.2s;
        box-sizing: border-box;
    }
    .search-button:hover {
        cursor: pointer;
        background-color: var(--medium-purple);
    }

    .search-button:active {
        margin-top: 2px;
    }
</style>