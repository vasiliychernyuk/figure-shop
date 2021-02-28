<template>
    <section class="first-look-section">
        <MainSidebar />
        <FirstLookContent />
    </section>
</template>

<script>
import MainSidebar from './main-sidebar/main-sidebar.vue';
import FirstLookContent from './first-look-content/first-look-content.vue';
export default {
    name: 'first-look-section',
    components: {
        MainSidebar,
        FirstLookContent
    }
}
</script>

<style src="./first-look-section.css"></style>