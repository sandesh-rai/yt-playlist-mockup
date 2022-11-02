<template>
  <div class="playlist-header-container">
        <div class="playlist-header-container--row">
            <div>
                <div></div>
                <img src="../assets/img/mountains-royalty-free.png" alt="header-mountain-image"/>
            </div>

            <header>
                <h2>Video Title Here</h2>
                <h4>Username123</h4>
                <p><span>40 videos</span> <span>Last updated on 25 December 2021</span></p>
            </header>
        </div>

        <div class="playlist-header-container--row" style="margin: 16px 0">
            <button class="button--play-all"><i class="fa-solid fa-play"></i>Play All</button>
            <button class="button--shuffle"><i class="fa-solid fa-shuffle"></i>Shuffle</button>
        </div>
  </div>
</template>

<script>
export default {
    name: "PlaylistHeader"
}
</script>

<style scoped>

div.playlist-header-container {
    padding: 24px;
    background: linear-gradient(to bottom, rgba(101, 104, 164, 0.800) 0%, rgba(48, 39, 52,0.298) 33.000001%, rgba(15,15,15,1.000) 100%);
}

div.playlist-header-container--row {
    display: flex;
    justify-content: center;
}

div.playlist-header-container--row > *:not(button), div.playlist-header-container--row > div > img {
    height: 190px;
    width: 336px;
    color: #fff;
}

div.playlist-header-container--row > button {
    width: auto;
}

div.playlist-header-container--row > div > img {
    border-radius: 10px;
}

div.playlist-header-container--row > header {
    padding-left: 24px;
}

div.playlist-header-container--row > header > h2 {
    font-size: 2.8rem;
    line-height: 3.8rem;
    font-weight: 700;
}

div.playlist-header-container--row > header > h4 {
    font-size: 1.4rem;
    line-height: 2rem;
    font-weight: 500;
}

div.playlist-header-container--row > header > p {
    font-size: 1.2rem;
    line-height: 1.8rem;
    font-weight: 400;
}

button.button--play-all, button.button--shuffle {
    font-size: 1.4rem;
    padding: 0 1.6rem;
    width: auto;
    font-weight: 500;
    flex-grow: 1;
    height: 3.6rem;
    letter-spacing: 0.5px;
    border-radius: 18px;
}

button.button--play-all > i, button.button--shuffle > i{
    margin-left: -6px;
    margin-right: 6px;
}
</style>