<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

<div class="new-post">
  <div class="post-box">
    <textarea class="post-text" placeholder="Share something here"></textarea>
  </div>
  <div class="post-info">
    <button class="post-button">POST</button>
  </div>
</div>

<style>
  .new-post {
    display: flex;
    flex-direction: column;
    min-width: 350px;
    width: 40vw;
    margin-bottom: 10px;
    box-sizing: border-box;
    border: 1.5px solid var(--border-grey);
    border-radius: 7px;
    box-shadow: 0 2px 1px var(--shadow-grey);
    background-color: white;
  }

  .post-box {
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 5px;
  }

  .post-text {
    min-width: 330px;
    width: 39vw;
    min-height: 100px;
    border: none;
    background-color: white;
    font-family: 'Roboto';
    font-size: 1rem;
    line-height: 1.5rem;
    resize: none;
  }

  .post-text:focus {
    outline: none;
  }

  .post-info {
    display: flex;
    align-items: center;
    justify-content: end;
    height: 30px;
    padding-bottom: 5px;
  }

  .post-button {
    padding: 5px 10px;
    margin-right: 10px;
    font-size: 1rem;
    border: none;
    border-radius: 5px;
    box-shadow: 0 2px 1px var(--shadow-grey);
    background-color: var(--dark-purple);
    color: white;
    transition: background-color 0.2s;
  }

  .post-button:hover {
    cursor: pointer;
    background-color: var(--hover-purple);
  }

  .post-button:active {
    margin-top: 2px;
  }

</style>