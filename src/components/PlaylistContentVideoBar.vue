<template>
    <button class="video-bar">
        <p>{{videoNumber}}</p>
        <img class="video-bar__thumbnail" src="../assets/img/mountains-royalty-free.png" alt="header-mountain-image"/>
        <div class="video-bar__video-data">
            <h5>{{`Example Title of Video Here ${videoNumber}`}}</h5>
            <a>Username123</a>
        </div>
    </button>
  
</template>

<script>
export default {
    name: "PlaylistContentVideoBar",
    props: {
        videoNumber: {
            type: Number
        }
    }

}
</script>

<style scoped lang="scss">
@import "../assets/scss/_main.scss";
button.video-bar {
    display: flex;
    padding: 8px 0px;
    border-radius: 10px;
    background-color: $base-dark-bg;  
    border: none;
}

button.video-bar:hover, button.video-bar:active, button.video-bar:focus-visible {
    background-color: rgba(255, 255, 255, 0.1);
}

button.video-bar > p {
    color: #fff;
    padding: 8px 14px 0px;
    font-weight: 500;
    font-size: 1.4rem;
    width: 1.4rem;
}

img.video-bar__thumbnail {
    max-width: 120px;
    border-radius: 10px;
    margin-right: 8px;
}

div.video-bar__video-data {
    display: flex;
    flex-direction: column;
    cursor: pointer;
    flex-grow: 1;
    margin-left: 8px;
}

div.video-bar__video-data > h5 {
    color: #fff;
    font-size: 1.6rem;
    font-weight: 500;
    margin: 0 0 8px;
    line-height: 2.2rem;
    max-height: 4.4rem;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: normal;
    text-align: left;
}

div.video-bar__video-data > a {
    color: #aaa;
    text-decoration: none;
    text-align: left;
    width: 0;
}

div.video-bar__video-data > a:hover {
    color: #fff
}

</style>