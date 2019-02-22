<template>
    <span class="c-menu-item-label"><slot>サンプル</slot></span>
</template>

<script lang="ts">
    import {Component, Vue} from "vue-property-decorator";

    @Component
    export default class MenuItemLabel extends Vue {
    }
</script>

<style scoped lang="scss">
    .c-menu-item-label {
        font-size: 12px;
    }
</style>
