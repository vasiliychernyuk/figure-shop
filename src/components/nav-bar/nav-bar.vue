<template>
    <nav>
        <NavBarLink 
            :key="idx" v-for="(value, idx) in navBarLinksTitles"
            :title="value.title"
            :src="value.src"
        />
    </nav>
</template>

<script>
import NavBarLink from './nav-bar-link/nav-bar-link.vue';

export default {
    name: 'nav-bar',
    components:{
        NavBarLink
    },
    data(){
        return{
            navBarLinksTitles: [
                {
                    title: 'Лидеры продаж',
                    src: '#'
                },
                {
                    title: 'Новинки',
                    src: '#'
                },
                {
                    title: 'Cеты',
                    src: '#'
                },
                {
                    title: 'Скидки',
                },
                {
                    title: 'Купоны'
                }
            ]
        }
    }
}
</script>

<style>
    nav{
        padding: .2rem 1rem;
        border-bottom: 1px solid rgba(0,0,0,.05);
    }
</style>