<script>
  import TrendingData from "./trendingData.svelte";
</script>

  <div class="trending-box">
      <TrendingData>
          <article slot="trend" let:topic class="trending-topic">
              {topic}
          </article>
      </TrendingData>
    </div>

<style>  

    .trending-box {
        display: flex;
        flex-direction: column;
        gap: 10px;
        width: 315px;
        border-radius: 5px;
        box-sizing: border-box;
    }

    .trending-topic {
        display: flex;
        align-items: center;
        padding-left: 10px;
        height: 40px;
        font-size: 1rem;
        border-radius: 5px;
        background-color: #37186C;
        color: white;
        transition: background-color 0.2s;
        box-sizing: border-box;
    }

    .trending-topic:hover {
        background-color: #6742A6;
        cursor: pointer;
    }

</style>