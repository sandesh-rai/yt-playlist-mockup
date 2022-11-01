<template>
    <button class="app-sidebar-button">
        <div class="app-sidebar-button--icon">
            <slot name="icon">
            </slot>
        </div>
        <span>{{title}}</span>
    </button>
</template>

<script>
export default {
    name: "AppSidebarButton",
    props: {
        title: {
            type: String
        }
    }
}
</script>

<style scoped lang="scss">
@import "../assets/scss/_main.scss";

button.app-sidebar-button {
    background-color: $button-dark-inactive;
    width: 100%;
    padding: 16px 0px 14px;
    border-radius: 10px;
    cursor: pointer;
}

button.app-sidebar-button:hover,  button.app-sidebar-button:active {
    background-color: $button-dark-active;
    width: 100%;
    padding: 16px 0px 14px;
}


button.app-sidebar-button * {
    color: $inactive-white;
    text-align: center;
}

button.app-sidebar-button > span {
    font-size: 10px;
}

div.app-sidebar-button--icon > i {
    margin-bottom: 6px;
    font-size: 24px;
}

</style>