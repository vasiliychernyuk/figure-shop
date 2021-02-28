<template>
    <li class="main-sidebar-element">
        <a href="#">
            {{ title }}
        </a>
    </li>
</template>

<script>
export default {
    name: 'main-sidebar-element',
    props: {
        title: String,
        url: String
    }
}
</script>

<style src="./main-sidebar-element.css"></style>