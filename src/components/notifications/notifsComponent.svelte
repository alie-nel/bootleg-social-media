<script>
    import NotifsData from "./notifsData.svelte"
    
    let hidden = false;
    
    const markRead = () => {
        hidden = !hidden;
    }
</script>

<NotifsData>
    <div id="notifs" slot="notifs" let:title let:content class="notifs" on:click={markRead}>
    
        <div class="notifs-head">
            <div id="unread" class="unread" class:hidden>
            </div>

            <div class="notifs-title">
                {title}
            </div>
        </div>

        <div class="notifs-mid">
            <div class="notifs-content">
                {content}
            </div>
        </div>

    </div>
</NotifsData>

<style>
    .notifs {
        display: flex;
        flex-direction: column;
        margin-bottom: 10px;
        width: 400px;
        box-sizing: border-box;
        transition: background-color 0.2s;
    }

    .notifs:hover {
        background-color: #e9e8ea;
        cursor: pointer;
    }

    .notifs-head {
        display: flex;
        align-items: center;
        height: 50px;
    }

    .unread {
        margin-left: 10px;
        width: 10px;
        height: 10px;
        border-radius: 5px;
        background-color: #6742A6;
    }

    .notifs-title {
        margin-left: 10px;
        font-size: 1rem;
        color: #47464a;
    }

    .notifs-mid {
        display: flex;
    }

    .notifs-content {
        padding: 15px 10px 25px 10px;
        color: #47464a;
        font-size: 0.9rem;
    }

    .hidden {
        display: none;
    }

</style>