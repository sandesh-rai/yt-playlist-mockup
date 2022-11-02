<template>
  <div class="playlist-header-container main-playlist-container">
        <div class="playlist-header-container--row playlist-header-container--row-top">
            <div class="playlist-image">
                <img src="../assets/img/mountains-royalty-free.png" alt="header-mountain-image"/>
                <div class="playlist-image-overlay"><i class="fa-solid fa-play"></i> PLAY ALL</div>
            </div>

            <header>
                <h2>Video Title Here</h2>
                <div class="playlist-header__meta-data-action-bar-container">
                    <div class="playlist-header__meta-data">
                        <h4>Username123</h4>
                        <p><span style="margin-right: 4px">20 videos </span><span>Last updated on 01 Nov 22</span></p>
                    </div>
                    <div class="playlist-header__action-bar">
                        <button class="button-transparent">
                            <i class="fa-solid fa-plus"></i>
                        </button>
                        <button class="button-transparent">
                            <i class="fa-solid fa-share"></i>
                        </button>
                        <button class="button-transparent">
                            <i class="fa-solid fa-ellipsis-vertical"></i>
                        </button>
                    </div>
                </div>
            </header>
        </div>

        <div class="playlist-header-container--row" style="margin-top: 16px; margin-bottom: 16px">
            <button class="button-white button--play-all"><i class="fa-solid fa-play"></i>Play All</button>
            <button class="button-transparent button--shuffle"><i class="fa-solid fa-shuffle"></i>Shuffle</button>
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
}

div.playlist-header-container--row {
    justify-content: space-between;
}

div.playlist-header-container--row > *:not(button), div.playlist-header-container--row > div > img {
    color: #fff;
    max-width: 350px;
    flex-grow: 1;
}

div.playlist-header-container--row > button {
    width: auto;
    cursor: pointer;
}

div.playlist-image {
    margin-top: auto;
    margin-bottom: auto;
    position: relative;
}

div.playlist-image:hover {
    background-color: #000;
    border-radius: 10px;
}

div.playlist-image > img {
    border-radius: 10px;
    width: 350px;
    height: 175px;
    cursor: pointer;
}

div.playlist-image:hover > img {
    opacity: 0.5;
}

div.playlist-image > div.playlist-image-overlay{
    opacity: 0;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    text-align: center;
    font-size: 1.4rem;
}

div.playlist-image:hover > div.playlist-image-overlay{
    opacity: 1;
}

div.playlist-header-container--row > header {
    padding-left: 24px;
    display: flex;
    flex-flow: column;
    justify-content: center;
}

div.playlist-header-container--row > header > h2 {
    font-size: 2.8rem;
    line-height: 3.8rem;
    font-weight: 700;
    margin: 12px 0;
}

div.playlist-header__meta-data-action-bar-container {
    margin-top: 16px 0px 12px;
    display: flex;
}

div.playlist-header__meta-data {
    flex-grow: 1;
}

div.playlist-header__meta-data > h4 {
    font-size: 1.4rem;
    line-height: 2rem;
    font-weight: 500;
    margin: 0 0 4px;
    cursor: pointer;
}

div.playlist-header__meta-data > p {
    font-size: 1.2rem;
    line-height: 1.8rem;
    font-weight: 400;
    margin: 0;
    color: rgba(255, 255, 255, 0.7);
}

div.playlist-header__action-bar {
    display: flex;
    align-items: flex-end;
}

div.playlist-header__action-bar > button {
    border-radius: 50%;
    height: 3.6rem;
    width: 3.6rem;
    margin-left: 8px;
    font-size: 1.8rem;
}

button.button-white {
    color: #000;
    background-color: #fff;
}

button.button-white:hover, button.button-white:active, button.button-white:focus-visible {
    background-color: #e6e6e6;
}

button.button-transparent {
    border: none;
    color: #fff;
    background-color: rgb(255, 255, 255, 0.1);
    cursor: pointer;
    outline: none;
}

button.button-transparent:hover, button.button-transparent:active, button.button-transparent:focus-visible  {
    background-color: rgba(255, 255, 255, 0.2);
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
    border: none;
}

button.button--play-all {
    margin-right: 4px;
}

button.button--shuffle {
    margin-left: 4px;
}


button.button--play-all > i, button.button--shuffle > i{
    margin-left: -6px;
    margin-right: 6px;
}

@media screen and (max-width: 720px){
    div.playlist-header-container--row-top {
        flex-direction: column;
    }

    div.playlist-image {
        margin: 0 auto 16px;
    }

    div.playlist-header-container--row > *:not(button):not(img) {
        max-width: none;
    }

    div.playlist-image > img {
        width: 100%;
    }

    div.playlist-header-container--row > header {
        margin: 0;
    }

}
</style>

<style>

div.main-playlist-container > * {
    max-width: 720px;
    display: flex;
    margin-left: auto;
    margin-right: auto;
}

</style>