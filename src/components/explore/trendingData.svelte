<script>
  const trendingData = [
      {
          topic: '#' + 'AI',
      },
      {
          topic: '#' + 'Concert tickets',
      },
      {
          topic: '#' + 'Controversy',
      },
      {
          topic: '#' + 'Meme',
      },
      {
          topic: '#' + 'Puppies',
      },
  ]

</script>

{#each trendingData as trend}
  <slot
      name="trend"
      topic = {trend.topic}
  />
{/each}