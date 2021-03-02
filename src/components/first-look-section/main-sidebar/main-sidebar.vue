<template>
    <aside class="main-sidebar-section">
        <ul class="main-sidebar-section__categories">
            <h4>
                <svg width="19" height="19" xmlns="http://www.w3.org/2000/svg">
                    <g>
                        <line stroke-linecap="null" stroke-linejoin="null" id="svg_10" y2="17.18041" x2="44.03608" y1="17.07732" x1="44.03608" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" stroke="#000" fill="none"/>
                        <line stroke="#333" stroke-linecap="null" stroke-linejoin="null" id="svg_13" y2="1.98387" x2="19.05735" y1="1.98387" x1="9.46201" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="null" stroke-width="4" fill="none"/>
                        <line stroke="#333" stroke-linecap="null" stroke-linejoin="null" id="svg_15" y2="9.5" x2="22.1129" y1="9.5" x1="9.04534" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="null" stroke-width="4" fill="none"/>
                        <line stroke="#333" stroke-linecap="null" stroke-linejoin="null" id="svg_16" y2="17" x2="22.1129" y1="17" x1="9.04534" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="null" stroke-width="4" fill="none"/>
                        <line stroke="#333" stroke-linecap="null" stroke-linejoin="null" id="svg_17" y2="2" x2="4.46774" y1="2" x1="-0.04839" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="null" stroke-width="4" fill="none"/>
                        <line stroke="#333" stroke-linecap="null" stroke-linejoin="null" id="svg_18" y2="9.5" x2="4.46774" y1="9.5" x1="-0.04839" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="null" stroke-width="4" fill="none"/>
                        <line stroke="#333" stroke-linecap="null" stroke-linejoin="null" id="svg_19" y2="17" x2="4.46774" y1="17" x1="-0.04839" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="null" stroke-width="4" fill="none"/>
                    </g>
                </svg>
                Категории
            </h4>
            <MainSidebarElement :key="idx" v-for="(item, idx) in titles" :title="item.title" :iconSVG="item.iconSVG" />
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
                { 
                    title:  'Круги',
                    iconSVG: '<svg width="19" height="19" xmlns="http://www.w3.org/2000/svg"><g><ellipse stroke-dasharray="5,2,2,2,2,2" stroke="#000" ry="8.95488" rx="8.95488" id="svg_1" cy="9.5" cx="9.5" fill="none"/></g></svg>'
                },
                { 
                    title: 'Квадраты',
                    iconSVG: '<svg width="19" height="19" xmlns="http://www.w3.org/2000/svg"><g><line fill="none" stroke="#000" stroke-width="null" stroke-dasharray="5,2,2,2,2,2" stroke-opacity="null" fill-opacity="null" opacity="undefined" x1="44.03608" y1="17.07732" x2="44.03608" y2="17.18041" id="svg_10" stroke-linejoin="null" stroke-linecap="null"/><rect id="svg_1" height="18.08916" width="18.08916" y="0.45542" x="0.45542" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" stroke="#000" fill="none"/></g></svg>'
                },
                { 
                    title: 'Треугольники',
                    iconSVG: '<svg width="19" height="19" xmlns="http://www.w3.org/2000/svg"><g><line stroke="#000" stroke-linecap="null" stroke-linejoin="null" id="svg_3" y2="18.46286" x2="0.30928" y1="0.43405" x1="9.69072" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" fill="none"/><line stroke="#000" stroke-linecap="null" stroke-linejoin="null" id="svg_4" y2="0.37629" x2="10.06701" y1="18.41752" x1="18.52062" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" fill="none"/><line stroke-linecap="null" stroke-linejoin="null" id="svg_5" y2="18.41752" x2="17.79897" y1="18.62371" x1="0.68557" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" stroke="#000" fill="none"/></g></svg>'
                },
                { 
                    title: 'Подставки под примитивы',
                    iconSVG: '<svg width="19" height="19" xmlns="http://www.w3.org/2000/svg"><g><line stroke-linecap="null" stroke-linejoin="null" id="svg_5" y2="18.41752" x2="17.79897" y1="18.62371" x1="0.68557" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" stroke="#000" fill="none"/><line stroke-linecap="null" stroke-linejoin="null" id="svg_6" y2="18.93299" x2="0.53093" y1="14.5" x1="0.53093" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" stroke="#000" fill="none"/><line stroke-linecap="null" stroke-linejoin="null" id="svg_7" y2="18.93299" x2="18.46907" y1="14.5" x1="18.46907" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" stroke="#000" fill="none"/><line stroke-linecap="null" stroke-linejoin="null" id="svg_9" y2="14.39691" x2="18.88259" y1="14.39691" x1="0.32474" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" stroke="#000" fill="none"/><line stroke-linecap="null" stroke-linejoin="null" id="svg_10" y2="17.18041" x2="44.03608" y1="17.07732" x1="44.03608" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" stroke="#000" fill="none"/><ellipse ry="6.49485" rx="6.49485" id="svg_11" cy="7.02577" cx="9.5" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" stroke="#000" fill="none"/></g></svg>'
                },
                {
                    title: 'Брелки для примитивов',
                    iconSVG: '<svg width="19" height="19" xmlns="http://www.w3.org/2000/svg"><g><line stroke-linecap="null" stroke-linejoin="null" id="svg_10" y2="17.18041" x2="44.03608" y1="17.07732" x1="44.03608" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" stroke="#000" fill="none"/><ellipse ry="5.56701" rx="5.56701" id="svg_12" cy="12.95361" cx="6.20103" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" stroke="#000" fill="none"/><path id="svg_13" d="m17.95361,0.68557c-8.24742,-0.82474 -11.4433,6.70103 -11.45876,6.63402" opacity="NaN" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" stroke="#000" fill="none"/><ellipse ry="1.08247" rx="1.08247" id="svg_14" cy="1.76804" cx="17.59278" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" stroke="#000" fill="none"/></g></svg>'
                },
                {
                    title: 'Прочие аксессуары',
                    iconSVG: '<svg width="19" height="19" xmlns="http://www.w3.org/2000/svg"><g><line stroke-linecap="null" stroke-linejoin="null" id="svg_10" y2="17.18041" x2="44.03608" y1="17.07732" x1="44.03608" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" stroke="#000" fill="none"/><ellipse ry="1.08247" rx="1.08247" id="svg_14" cy="4.44845" cx="4.91237" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" stroke="#000" fill="none"/><line stroke="#000" stroke-linecap="null" stroke-linejoin="null" id="svg_15" y2="10.47938" x2="14.55155" y1="5.32474" x1="14.55155" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" fill="none"/><line stroke-linecap="null" stroke-linejoin="null" id="svg_16" y2="7.90206" x2="17.23196" y1="7.79897" x1="11.97423" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" stroke="#000" fill="none"/><rect stroke="#000" id="svg_17" height="4.75186" width="4.44625" y="11.30412" x="5.2732" opacity="undefined" fill-opacity="null" stroke-opacity="null" stroke-dasharray="5,2,2,2,2,2" stroke-width="null" fill="none"/></g></svg>'
                }
            ]
        }
    },
    components: {
        MainSidebarElement
    }
}
</script>

<style src="./main-sidebar.css"></style>