<template>
    <li class="main-sidebar-element">
        <a href="#">
            <SidebarIcon :iconSVG="iconSVG"/>
            {{ title }}
        </a>
    </li>
</template>

<script>
import SidebarIcon from './main-sidebar-element-icon/main-sidebar-element-icon.vue';
export default {
    name: 'main-sidebar-element',
    props: {
        title: String,
        url: String,
        iconSVG: String
    },
    components: {
        SidebarIcon
    }
}
</script>

<style src="./main-sidebar-element.css"></style>