<template>
    <footer class="c-footer">
        <FooterNavigation />
    </footer>
</template>

<script lang="ts">
    import {Component, Vue} from 'vue-property-decorator';
    import FooterNavigation from '../molecules/FooterNavigation';
    @Component({
        components: {FooterNavigation}
    })
    export default class Footer extends Vue {
    }
</script>

<style scoped>

</style>
