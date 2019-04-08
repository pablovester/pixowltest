<template>
    <div id="app">
        <Bar />
        <MainHeader />
        <Section v-bind:info="firsttitlesubtitle" v-bind:list="firstcontent" v-bind:images="contentfirstimage" />
        <Section v-bind:info="secondtitlesubtitle" v-bind:list="secondcontent" v-bind:images="contentsecondimage" />
        <Footer />
    </div>
</template>
<script>
import Bar from './components/Bar.vue'
import MainHeader from './components/MainHeader.vue'
import Section from './components/Section.vue'
import Footer from './components/Footer.vue'


export default {
    name: 'app',
    components: {
        Bar,
        MainHeader,
        Section,
        Footer
    },


    data() {
        return {

            firsttitlesubtitle: [
                { title: 'Powerful easy to use modeling tools' },
                { subtitle: 'Make the most of your creativity with a robust set of tools. If you are an advanced 3D modeler or just starting out, with our super user-friendly interface you will creating amazing stuff right away.' }
            ],

            secondtitlesubtitle: [
                { title: 'Animate your creations' },
                { subtitle: 'A game changer in the voxel word. With our own Skeleton System, VoxEditor allows you to rig and animate anything that you want using the timeline with a super easy to use keyframing mode.' }
            ],


            contentfirstimage: [
                '/assets/img2.png'
            ],

            contentsecondimage: [
                '/assets/img3.png'
            ],

            firstcontent: [
                'All in one software with incredible performance',
                'Windows and Mac supported',
                'Amazing voxel creation tools',
                'Emisive Wand. Make your work glow',
                'Increase your voxels to get that level of detail',
                'Work with a big Canvas',
                'Mirror XYZ. Work less, we take care of the rest',
                'Voxel, Quads and super fast Render view',
                'Advanced Color Palette',
                'Super friendly 3D enviroment to work',
                'And much more'
            ],

            secondcontent: [
                'Animation! Bring your creation to life',
                'Skeleton System',
                'Cut & Rig',
                'Powerful Timeline',
                'Keyframing interpolation',
                'Curves',
                'Animations integrated in one file'
            ]
        }
    }

}
</script>
<style>
html {
    scroll-behavior: smooth;
}

#app {
    font-family: 'Montserrat', sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    margin: 0;
    background-color: black;
}

body {
    margin: 0;
}

h1 {
    font-weight: 700;
    text-transform: uppercase;
}

h3,
li {
    font-weight: 500;
}

.nomargin {
    margin: 0;
}

.white {
    color: white;
}

div#content.section {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
}

div#content.section:nth-of-type(2n+1) {
    background-color: #151619;
    overflow: hidden;
    clip-path: polygon(0 0, 100% 10%, 100% 90%, 0 100%);
    display: flex;
    justify-content: center;
    align-items: center;
}

div#content.section:nth-of-type(2n) {
    flex-direction: row-reverse;
    margin-left: 5%;
}

div#content.section:nth-of-type(2n+1)>.text-container {
    margin-left: 5%;
}

div#content.section:nth-of-type(2n)>.text-container {
    margin-right: 5%;
}

@media (orientation: portrait) {

    div#content.section:nth-of-type(2n+1),
    div#content.section:nth-of-type(2n) {
        flex-direction: column;
        min-height: 150vh;
    }
}
</style>