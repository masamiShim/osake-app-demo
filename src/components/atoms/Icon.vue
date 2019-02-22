<template>
    <i class="fa-2x" :class="icon"></i>
</template>

<script lang="ts">
    import {Component, Prop, Vue} from "vue-property-decorator";

    @Component
    export default class Icon extends Vue {
        @Prop() private icon!: string;
    }
</script>

<style scoped>
</style>
