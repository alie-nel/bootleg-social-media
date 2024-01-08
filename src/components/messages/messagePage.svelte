<script>
    import MessageComponent from "./messageComponent.svelte"
</script>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

    <section class="messages-section">

        <h1 class="messages-title">Messages</h1>

        <MessageComponent />
        
    </section>

<style>
    .messages-section {
        margin-left: 200px;
        width: 410px;
        height: 100vh;
        border-right: 1px solid #a7a8a4;
        font-family: 'Roboto', sans-serif;
    }

    .messages-title {
        margin-left: 10px;
        color: var(--dark-purple);
    }

</style>