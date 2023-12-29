<template>
    <div id="main-3-container">
        <div class="main-3-holder"></div>
        <div class="main-3-holder"></div>
        <div class="main-3-holder"></div>
    </div>

</template>

<script>
export default {
    name: " mainThree",
}
</script>

<style scoped>
#main-3-container {
    width : 100vw;
    height : 60vh;
    background-color: rgb(202, 45, 45);
    display : flex;
    justify-content: center;
    align-items: center;
    align-content: center;
}

.main-3-holder {
    border-color: white;
    border-width: 3px;
    border-style : solid;
    width  : 27vw;
    height : 40vh;
    margin: 20px;
}
</style>