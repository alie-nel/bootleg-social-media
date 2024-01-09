<script>
  const profileData = {
    user: 'sheeky22',
    bio: 'Welcome to my page!',
    followers: 46,
    following: 754,
  }
</script>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

  <div class="profile-banner">
    <div class="profile-pic"></div>
    <h3 class="username">{profileData.user}</h3>
    <p class="bio">{profileData.bio}</p>

    <div class="numbers">
      <p class="followers">Followers</p>
          <p class="tweet-num">
              {profileData.followers}
          </p>
      <p class="following">Following</p>
          <p class="tweet-num">
              {profileData.following}
          </p>
    </div>
  </div>

<style>
  .profile-banner {
      display: flex;
      flex-direction: column;
      margin-bottom: 20px;
      box-sizing: border-box;
    }
  
  .profile-pic {
      width: 80px;
      height: 80px;
      border-radius: 40px;
      background-color: var(--medium-purple);
  }

    .username {
    }

    .bio {
        font-size: 0.9rem;
    }

    .numbers {
        display: flex;
        gap: 5px;
        font-size: 0.9rem;
        font-weight: bold;
    }

    .tweet-num {
        font-weight: normal;
        margin-right: 5px;
    }

    .followers:hover {
        text-decoration: underline;
        cursor: pointer;
    }

    .following:hover {
        text-decoration: underline;
        cursor: pointer;
    }
</style>