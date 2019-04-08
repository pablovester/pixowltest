<template>
    <div id="footer">
        <div id="main-footer">
            <img src="/assets/sandboxlogo.png" />
            <div id="pages-container" class="white">
                <h1>Pages</h1>
                <div id="list-pages-container">
                    <div id="column-one">
                        <ul v-for="item in footerlistone">
                            <li>{{item}}</li>
                        </ul>
                    </div>
                    <div id="column-two">
                        <ul v-for="item in footerlisttwo">
                            <li>{{item}}</li>
                        </ul>
                    </div>
                </div>
            </div>
            <div id="social-container" class="white">
                <h1>Social</h1>
                <img v-for="image in mediaicons" :src="image" />
            </div>
        </div>
        <div id="copyright-footer">
            <p v-text="copyright"></p>
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {

            footerlistone: [
                'News',
                'Create',
                'Marketplace',
                'Game'
            ],

            footerlisttwo: [
                'Editor',
                'Whitepaper',
                'Team',
                'FAQ'
            ],

            mediaicons: [
                '/assets/medium.png',
                '/assets/discord.png',
                '/assets/pixowl.png'
            ],

            copyright: 'Copyright © 2012-2018, The Sandbox. All Rights Reserved.'

        }
    }
}
</script>
<style>
#footer {
    background-color: #151619;
}

#main-footer {
    display: flex;
    justify-content: space-evenly;
    margin: 3%;
}

#main-footer img {
    align-self: center;
}

#copyright-footer {
    background-color: #242527;
    height: 2rem;
    text-align: center;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #505052;
}

#copyright-footer p {
    margin: 0;
}

h1 {
    font-size: 1.5rem;
}

#list-pages-container {
    display: flex;
}

#pages-container {
    width: 25%;
}

#column-one {
    margin-right: 10%;
}

#column-two {
    margin-left: 10%;
}

ul {
    list-style: none;
    margin: 0;
    padding: 0;
}

li,
#copyright-footer p {
    font-size: 0.8rem;
}

@media (orientation: portrait) {

    #main-footer {
        flex-direction: column;
        align-items: center;
    }

    #main-footer img {
        margin-top: 10%;
    }

    #pages-container {
        width: auto;
    }
}
</style>