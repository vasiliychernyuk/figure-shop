<template>
    <div class="main-search-inp-section">

        <div class="main-search-inp-section__input">
            <input type="text">
            <button>
                <SearchIcon />
            </button>
        </div>
        
    </div>
</template>

<script>
import SearchIcon from './main-search-inp-icon/main-search-inp-icon.vue';
export default {
    name: 'main-search-input',
    components:{
        SearchIcon
    }
}
</script>
<style src="./main-search-input.css"></style>