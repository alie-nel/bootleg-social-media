<script>
    import ProfileBanner from "./profileBanner.svelte";
    import NewPost from "../newPost.svelte"
    import TweetComponent from "./tweetComponent.svelte"
</script>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

    <section class="profile-section">

        <h1 class="profile-title">Profile</h1>
        <ProfileBanner />
        <NewPost />
        <h3 class="posts-title">Posts</h3>
        <TweetComponent />
        
    </section>

<style>
    .profile-section {
        font-family: 'Roboto', sans-serif;
    }

    .profile-title {
        color: var(--dark-purple);
    }

    .posts-title {
        color: var(--dark-purple);
    }

</style>