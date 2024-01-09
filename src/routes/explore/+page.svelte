<script>
  import NavBar from "../../components/navBar.svelte"
  import ExplorePage from "../../components/explore/explorePage.svelte"
</script>

<NavBar />

<div class="explore-page">
  <ExplorePage/>
</div>

<style>
  .explore-page {
    display: flex;
    margin-left: 17vw;
  }

  @media (max-width: 550px) {
    .explore-page {
        justify-content: center;
    }
  }

</style>