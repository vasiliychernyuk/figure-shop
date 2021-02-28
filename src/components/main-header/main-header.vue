<template>
    <header>
        <Logo />
        <Search />
    </header>
</template>

<script>
import Logo from './web-site-logo/web-site-logo.vue';
import Search from './main-search-inp/main-search-input.vue'

export default {
    name: 'main-header',
    components: {
        Logo,
        Search
    }
}
</script>

<style>
    header{
        display: grid;
        grid-template-columns: 4fr 4fr 4fr;
        grid-template-areas: "main-header-logo main-header-inp main-header-others";

        height: 7rem;
        background-color: rgba(0,0,0,.02);
    }
</style>