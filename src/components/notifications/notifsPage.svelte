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
        margin-left: 200px;
        width: 410px;
        border-right: 1px solid #a7a8a4;
        font-family: 'Roboto', sans-serif;
    }

    .notifs-title {
        margin-left: 10px;
        color: #47464a;
    }

</style>