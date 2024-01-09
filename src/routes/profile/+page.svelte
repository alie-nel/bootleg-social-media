<script>
    import NavBar from "../../components/navBar.svelte"
    import ProfilePage from "../../components/profile/profilePage.svelte"
    import ExplorePage from "../../components/explore/explorePage.svelte"
</script>

<NavBar />

<div class="profile-page">
    <ProfilePage />
    <div class="explore-page">
        <ExplorePage />
    </div>
</div>

<style>
    .profile-page {
        display: flex;
        gap: 7vw;
        margin-left: 17vw;
    }

    @media (max-width: 750px) {
        .profile-page {
            justify-content: center;
        }
    }

    @media (max-width: 750px) {
        .explore-page {
            display: none;
        }
    }

</style>