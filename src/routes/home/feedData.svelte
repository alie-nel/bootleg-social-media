<script>
    const tweetData = [
        {
            user: '@' + '__erastime',
            content: 'I COULD NOT GET TAYLOR SWIFT TICKETS I CANNOT DO THIS ANYMORE',
            likes: 45,
            comments: 5,
            retweets: 123
        },
        {
            user: '@' + 'wishywashy21',
            content: "You know, every time I see a spider, my inner biologist and arachnophobe have a little showdown. On one hand, I'm amazed by their web-spinning skills, but on the other, I'm doing the 'spider dance' like a true champion of arachnophobia!",
            likes: 70,
            comments: 10,
            retweets: 47
        }
    ]

</script>

{#each tweetData as tweet (tweet)}
    <slot name="tweet" user={tweet.user} content={tweet.content} likes={tweet.likes} comments={tweet.comments} retweets={tweet.retweets} />
{/each}