<script>
    import NotifsComponent from "./notifsComponent.svelte"

</script>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

    <section class="notifs-section">

        <h1 class="notifs-title">Notifications</h1>

        <NotifsComponent />
        
    </section>

<style>
    .notifs-section {
        height: 100vh;
        width: 410px;
        border-right: 1px solid var(--border-grey);
        font-family: 'Roboto', sans-serif;
    }

    .notifs-title {
        margin-left: 10px;
        color: var(--dark-purple);
    }

    @media (max-width: 600px) {
        .notifs-section {
            width: 360px;
            border-right: none;
        }
    }

</style>