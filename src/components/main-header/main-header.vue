<template>
    <header>
        <Logo />
    </header>
</template>

<script>
import Logo from './web-site-logo/web-site-logo.vue';

export default {
    name: 'main-header',
    components: {
        Logo,
    }
}
</script>

<style>
    header{
        display: flex;
        justify-content: center;
    }
</style>