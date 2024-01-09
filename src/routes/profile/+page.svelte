<script>
    import NavBar from "../../components/navBar.svelte"
    import ProfilePage from "../../components/profile/profilePage.svelte"
    import ExplorePage from "../../components/explore/explorePage.svelte"
</script>

<div class="profile-page">
    <NavBar />
    <ProfilePage />
    <ExplorePage />
</div>

<style>
    .profile-page {
        display: flex;
    }
</style>