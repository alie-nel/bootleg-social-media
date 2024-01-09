<script>
    import NavBar from "../../components/navBar.svelte"
    import NotifsPage from "../../components/notifications/notifsPage.svelte"
</script>

<NavBar />

<div class="notifs-page">
    <NotifsPage />
</div>

<style>
    .notifs-page {
        display: flex;
        margin-left: 17vw;
    }

    @media (max-width: 600px) {
        .notifs-page {
            justify-content: center;
        }
    }
</style>