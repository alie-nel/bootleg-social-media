<script>
    const tweetData = [
        {
            user: '@' + 'sheeky22',
            content: 'Guys my dog fell into the toilet....',
            likes: 6,
            comments: 2,
            retweets: 1
        },
        {
            user: '@' + 'sheeky22',
            content: 'Whoever that guy is who cut in line yesterday.... I will find u',
            likes: 3,
            comments: 0,
            retweets: 0
        }
    ]

</script>

{#each tweetData as tweet (tweet)}
    <slot name="tweet" user={tweet.user} content={tweet.content} likes={tweet.likes} comments={tweet.comments} retweets={tweet.retweets} />
{/each}