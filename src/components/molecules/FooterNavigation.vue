<template>
    <nav class="c-footer-navigation">
        <ul class="c-footer-menu">
            <FooterMenuItem :icon="'fas fa-user-clock'" :label="'タイムライン'" />
            <FooterMenuItem :icon="'fas fa-search'" :label="'お店を検索'" />
            <FooterMenuItem :icon="'fas fa-utensils'" :label="'料理から選ぶ'" />
            <FooterMenuItem :icon="'far fa-user'" :label="'マイページ'" />
            <FooterMenuItem :icon="'fas fa-ellipsis-h'" :label="'その他'" />
        </ul>
    </nav>
</template>

<script lang="ts">
    import { Component, Vue} from 'vue-property-decorator';
    import FooterMenuItem from './FooterMenuItem';
    @Component({
        components: {FooterMenuItem}
    })
    export default class FooterMenuList extends Vue {
    }
</script>

<style scoped lang="scss">
    ul {
        padding: 0;
        margin: 0;
    }
    .c-footer-menu{
        width: 95%;
        display: inline-flex;
        justify-content: space-between;
    }
    .c-footer-navigation {
    }
</style>
