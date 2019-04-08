<template>
    <div id="content" class="section">
        <img :src="images">
        <div class="text-container">
            <div v-for="texts in info">
                <h1 class="white">{{texts.title}}</h1>
                <h3>{{texts.subtitle}}</h3>
            </div>
            <h2>features</h2>
            <ul>
                <li v-for="texts in list" class="white">{{texts}}</li>
            </ul>
        </div>
    </div>
</template>
<script>
export default {
    props: ['info', 'list', 'images'],
    data() {
        return {}
    }
}
</script>
<style scoped>
img {
    width: 100%;
    margin: 5%
}

h1 {
    font-size: 2rem;
    margin-bottom: 0;
}

h3 {
    font-size: 1rem;
    color: #b2b5b7
}

h2 {
    font-size: 1.5rem;
    color: #fe6b20;
    text-transform: uppercase;
    margin: 5% 0 0 0;
}

ul {
    list-style: none;
    padding: 0;
}

li {
    margin-bottom: 0.3em;
    padding-left: 1rem;
    position: relative;
    font-size: 0.8rem;
}

li:after {
    content: '';
    height: .4em;
    width: .4em;
    background: white;
    display: block;
    position: absolute;
    transform: rotate(45deg);
    top: .25em;
    left: 0;
}
</style>