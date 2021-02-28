<template>
    <aside class="main-sidebar-section">
        <ul class="main-sidebar-section__list">
            <MainSidebarElement :key="idx" v-for="(title, idx) in titles" :title="title" />
        </ul>
    </aside>
</template>

<script>
import MainSidebarElement from "./main-sidebar-element/main-sidebar-element.vue";
export default {
    name: 'main-sidebar',
    data(){
        return{
            titles: [
                'Круги',
                'Квадраты',
                'Треугольники',
                'Подставки под фигуры',
                'Брелки для фигур',
                'Дома для фигур',
                'Прочие аксессуары'
            ]
        }
    },
    components: {
        MainSidebarElement
    }
}
</script>

<style src="./main-sidebar.css"></style>