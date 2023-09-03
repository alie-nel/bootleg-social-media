<script>
    import TweetComponent from "../tweetComponent.svelte"
</script>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

    <section class="home-section">

        <h1 class="home-title">Profile</h1>
        
        <div class="profile-banner">
            <div class="profile-pic"></div>
            <h3 class="username">sheeky22</h3>
            <p class="bio">Welcome to my page!</p>
            <div class="numbers">
                <p class="followers">Followers</p>
                    <p class="tweet-num">
                        46
                    </p>
                <p class="following">Following</p>
                    <p class="tweet-num">
                        46
                </p>
            </div>

        </div>

        <h3 class="posts-title">Posts</h3>
        <TweetComponent />
        
    </section>

<style>
    .home-section {
        position: absolute;
        top: 0;
        left: 0;
        margin-left: 200px;
        padding-bottom: 20px;
        width: 600px;
        font-family: 'Roboto', sans-serif;
    }

    .home-title {
        position: relative;
        margin: 0;
        margin-top: 20px;
        margin-bottom: 40px;
        margin-left: 20px;
        color: #47464a;
    }

    .profile-banner {
        display: block;
        height: 130px;
    }
    
    .profile-pic {
        width: 80px;
        height: 80px;
        border-radius: 40px;
        background-color: green;
        margin-left: 20px;
    }

    .username {
        margin-left: 20px;
    }

    .bio {
        margin-left: 20px;
        font-size: 14px;
    }

    .numbers {
        display: flex;
        margin-top: -10px;
        margin-left: 20px;
        font-size: 14px;
        font-weight: bold;
    }

    .tweet-num {
        font-weight: normal;
        margin-left: 5px;
        margin-right: 10px;
    }

    .followers:hover {
        text-decoration: underline;
    }

    .following:hover {
        text-decoration: underline;
    }

    .posts-title {
        position: relative;
        margin: 0;
        margin-top: 100px;
        margin-left: 20px;
        color: #47464a;
    }

</style>