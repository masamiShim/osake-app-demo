<template>
    <li class="c-footer-menu-item">
        <div>
            <Icon class="l-footer-icon" :icon="icon" />
        </div>
        <div>
            <MenuItemLabel>{{ label }}</MenuItemLabel>
        </div>
    </li>
</template>

<script lang="ts">
    import {Vue, Component, Prop} from 'vue-property-decorator'
    import MenuItemLabel from '../atoms/MenuItemLabel';
    import Icon from '../atoms/Icon';

    @Component({
        components: {MenuItemLabel, Icon}
    })

    export default class FooterMenuItem extends Vue {
        @Prop({required: true})
        private icon!: string;

        @Prop({required: true})
        private label!: string;

    }
</script>

<style scoped lang="scss">
    .c-footer-menu-item {
        list-style: none;
    }
    .l-footer-icon {
        padding-right: 5px;
    }
</style>
