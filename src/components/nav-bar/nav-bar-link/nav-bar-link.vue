<template>
    <a class="nav-bar-link" :href="src">
        {{ title }}
    </a>
</template>

<script>
export default {
    name: 'nav-bar-link',
    props: {
        title: String,
        src: String
    }
}
</script>

<style src="./nav-bar-link.css"></style>