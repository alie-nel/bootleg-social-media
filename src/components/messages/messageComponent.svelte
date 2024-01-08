<script>
    import MessageData from "./messageData.svelte"
    
</script>

<MessageData>
    <article slot="message" let:user let:content class="message">
    
        <div class="message-head">
            <div class="message-pic">

            </div>
        
            <div class="message-user">
            {user}
            </div>
        </div>

        <div class="message-mid">
            <div class="message-content">
                {content}
            </div>
        </div>

    </article>
</MessageData>

<style>
    .message {
        display: flex;
        flex-direction: column;
        margin-bottom: 10px;
        width: 400px;
        box-sizing: border-box;
        background-color: white;
        transition: background-color 0.2s;
    }

    .message:hover {
        background-color: #e9e8ea;
        cursor: pointer;
    }

    .message-head {
        display: flex;
        align-items: center;
        height: 50px;
    }

    .message-pic {
        margin-left: 10px;
        width: 35px;
        height: 35px;
        border-radius: 20px;
        background-color: #6742A6;
    }

    .message-user {
        margin-left: 10px;
        font-size: 1rem;
        color: #47464a;
    }

    .message-mid {
        display: flex;
    }

    .message-content {
        padding: 15px 10px 25px 10px;
        margin-bottom: 5px;
        font-size: 0.9rem;
        color: #47464a;
    }

</style>