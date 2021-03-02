<template>
    <figure class="sidebar-element-icon" v-html="iconSVG"></figure>
</template>
<script>
export default {
    name: 'sidebar-element-icon',
    props: {
        iconSVG: String
    }
}
</script>
<style>
    .sidebar-element-icon{
        margin-right: .5rem;
    }
    
</style>