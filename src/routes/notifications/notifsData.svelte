<script>
    const notifsData = [
        {
            user: 'Recommended for you',
            content: 'You have liked 3 posts related to arachnids. Explore more like these here',
        },
        {
            user: 'News',
            content: "Elon Musk has just announced his newest venture. Click here to see more",
        }
    ]

</script>

{#each notifsData as notifs (notifs)}
    <slot name="notifs" user={notifs.user} content={notifs.content} />
{/each}