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
    background-color: transparent;
}

button.app-sidebar-button * {
    color: $inactive-white;
    text-align: center;
}

button.app-sidebar-button--icon {
    margin-bottom: 6px;
}

</style>