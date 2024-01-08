<script>
    const notifsData = [
        {
            title: 'Recommended for you',
            content: 'You have liked 3 posts related to arachnids. Explore more like these here',
        },
        {
            title: 'News',
            content: "Elon Musk has just announced his newest venture. Click here to see more",
        }
    ]

</script>

{#each notifsData as notifs (notifs)}
    <slot name="notifs" title={notifs.title} content={notifs.content} />
{/each}