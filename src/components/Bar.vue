<template>
    <div id="bar">
        <div id="triangle-container">
            <img src="/assets/voxlogo.png">
        </div>
        <div id="btn-container">
            <div class="btn">{{ btntxt }}</div>
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            btntxt: "DOWNLOAD"
        }
    }
}
</script>
<style>
#bar {
    height: 1.25rem;
    width: 100%;
    background-color: #151619;
    height: 4rem;
    display: flex;
    align-items: center;
}

#btn-container {
    display: flex;
    width: 60%;
    justify-content: flex-start;
}

.btn {
    border-radius: 10px;
    background-color: #3abeef;
    width: 10rem;
    height: 2.5rem;
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    font-weight: 800;
}

#triangle-container {
    width: 40%;
}

#triangle-container img {
    margin-top: 10%;
}

@media (orientation: portrait) {
    #triangle-container {
        width: 30%;
    }

    #triangle-container img {
        margin-top: 10%;
        width: 50%;
    }
}
</style>