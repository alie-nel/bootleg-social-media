<script>
    import TweetData from "./tweetData.svelte"
</script>

<TweetData>
    <article slot="tweet" let:user let:content let:likes let:comments let:retweets class="tweet">
    
        <div class="tweet-head">
            <div class="tweet-pic">
            </div>
        
            <div class="tweet-user">
            {user}
            </div>
        </div>

        <div class="tweet-mid">
            <div class="tweet-content">
                {content}
            </div>
        </div>

        <div class="tweet-end">
            
            <button class="tweet-icon">
                <i class="fa fa-thumbs-o-up"></i>
            </button>
            <p class="tweet-num">
                {likes}
            </p>
            
            <button class="tweet-icon">
                <i class="fa fa-comment"></i>
            </button>
            <p class="tweet-num">
                {comments}
            </p>

            <button class="tweet-icon">
                <i class="fa fa-retweet"></i>
            </button>
            <p class="tweet-num">
                {retweets}
            </p>
        </div>

    </article>
</TweetData>

<style>
    .tweet {
        display: flex;
        flex-direction: column;
        min-width: 350px;
        width: 40vw;
        margin-bottom: 10px;
        box-sizing: border-box;
        border: 1.5px solid #a7a8a4;
        border-radius: 5px;
        box-shadow: 0 2px 1px #ebe7e7;
        background-color: white;
    }

    .tweet-head {
        display: flex;
        align-items: center;
        gap: 7px;
        height: 50px;
        margin-left: 5px;
    }

    .tweet-pic {
        background-color: var(--medium-purple);
        width: 40px;
        height: 40px;
        border-radius: 20px;
    }

    .tweet-user {
        color: #47464a;
    }

    .tweet-mid {
        min-height: 50px;
        padding: 15px 10px;
        border-top: 1px solid #a7a8a4;
        border-bottom: 1px solid #a7a8a4;
    }

    .tweet-content {
        color: #47464a;
        font-size: 15px;
    }

    .tweet-end {
        display: flex;
        align-items: center;
        gap: 10px;
        margin-left: 5px;
        height: 40px;
    }

    .tweet-icon {
        width: 20px;
        height: 20px;
        border: none;
        border-radius: 5px;
        background-color: white;
        color: #37186C;
        transition: color 0.2s;
    }

    .tweet-icon:hover {
        cursor: pointer;
        color: #78619E;
    }

    .tweet-icon:active {
        margin-top: 2px;
    }

    .tweet-num {
        font-size: 14px;
        color: #47464a;
    }
</style>