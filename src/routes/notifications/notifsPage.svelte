<script>
    import NotifsComponent from "./notifsComponent.svelte"
</script>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

    <section class="notifs-section">

        <h1 class="notifs-title">Notifications</h1>

        <NotifsComponent />
        
    </section>

<style>
    .notifs-section {
        position: absolute;
        top: 0;
        left: 0;
        bottom: 0;
        margin-left: 200px;
        padding-bottom: 20px;
        width: 410px;
        border-right: 1px solid #a7a8a4;
        font-family: 'Roboto', sans-serif;
    }

    .notifs-title {
        position: relative;
        margin: 0;
        margin-top: 20px;
        margin-left: 20px;
        margin-bottom: 20px;
        color: #47464a;
    }

</style>