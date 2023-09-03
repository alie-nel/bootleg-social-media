<script>
    import NotifsData from "./notifsData.svelte"
    
</script>

<NotifsData>
    <article slot="notifs" let:user let:content class="notifs">
    
        <div class="notifs-head">
            <div class="unread">

            </div>

            <div class="notifs-user">
            {user}
            </div>
        </div>

        <div class="notifs-mid">
            <div class="notifs-content">
                {content}
            </div>
        </div>

    </article>
</NotifsData>

<style>
    .notifs {
        margin-top: 15px;
        margin-bottom: 10px;
        margin-left: 10px;
        padding-bottom: 5px;
        width: 400px;
        height: 100px;
        background-color: white;
        transition: background-color 0.2s;
    }

    .notifs:hover {
        background-color: #e9e8ea;
        cursor: pointer;
    }

    .notifs-head {
        display: flex;
        position: absolute;
        width: 400px;
        height: 50px;
    }

    .unread {
        position: relative;
        background-color: #6742A6;
        margin-top: 22px;
        margin-left: 10px;
        width: 10px;
        height: 10px;
        border-radius: 5px;
    }

    .notifs-user {
        position: relative;
        padding-top: 17px;
        margin-left: 10px;
        color: #47464a;
    }

    .notifs-mid {
        margin-top: 50px;
        position: absolute;
        display: block;
        width: 550px;
    }

    .notifs-content {
        position: relative;
        margin-top: 10px;
        margin-bottom: 5px;
        margin-left: 12px;
        margin-right: 15px;
        width: 360px;
        height: 100px;
        color: #47464a;
        font-size: 14px;
    }

</style>