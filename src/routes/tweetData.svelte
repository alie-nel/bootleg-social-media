<script>
    const tweetData = [
        {
            user: '@' + 'sheeky22',
            content: 'Guys my dog fell into the toilet....',
            likes: 45,
            comments: 5,
            retweets: 100
        },
        {
            user: '@' + 'sheeky22',
            content: 'Whoever that guy is who cut in line yesterday.... I will find u',
            likes: 45,
            comments: 5,
            retweets: 100
        }
    ]

</script>

{#each tweetData as tweet (tweet)}
    <slot name="tweet" user={tweet.user} content={tweet.content} likes={tweet.likes} comments={tweet.comments} retweets={tweet.retweets} />
{/each}