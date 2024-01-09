<script>
    import NavBar from "../../components/navBar.svelte"
    import MessagePage from "../../components/messages/messagePage.svelte"
</script>

<NavBar />

<div class="message-page">
    <MessagePage />
</div>

<style>
    .message-page {
        display: flex;
        margin-left: 17vw;
    }

    @media (max-width: 600px) {
        .message-page {
            justify-content: center;
        }
    }
</style>