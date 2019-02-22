<template>
    <div>
        <header class="c-header">
            <nav class="c-top-navigation">
                <ul class="c-top-menu">
                    <li class="c-top-menu-item"></li>
                    <li class="c-top-menu-item"></li>
                    <li class="c-top-menu-item"></li>
                    <li class="c-top-menu-item"></li>
                </ul>
            </nav>
        </header>
        <main class="c-main-content">
            <div class="c-main-content-wrapper">
                <section class="main-content"></section>
            </div>
        </main>
        <Footer />
    </div>
</template>

<script lang="ts">
    import {Component, Prop, Vue} from "vue-property-decorator";
    import Footer from './organisms/Footer';
    @Component({
        components: {Footer}
    })
    export default class HelloWorld extends Vue {
        @Prop() private msg!: string;
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    h3 {
        margin: 40px 0 0;
    }

    ul {
        list-style-type: none;
        padding: 0;
    }

    li {
        display: inline-block;
        margin: 0 10px;
    }

    a {
        color: #42b983;
    }
</style>
