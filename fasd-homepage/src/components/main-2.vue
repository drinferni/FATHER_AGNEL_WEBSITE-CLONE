
import { setBlockTracking } from 'vue';
<template>
    <div id="main-2-container"> 
        <div id="scroller-1">
            <div class="heading">Circulars</div>
            <div class="scroller"></div>
        </div>
        <div id="scroller-2">
            <div class="heading">Achievements</div>
            <div class="scroller"></div>
        </div>
        <div id="scroller-3">
            <div class="heading">Latest News</div>
            <div class="scroller"></div>
        </div>
    </div>

</template>





<script>
export default {
    name:"mainTwo",
    data () {
        return {
            scroll_data : {
                1 : ["aaaaaaaa","aaaaaaa","aaaaaa","aaaaaaaa","aaaaaaaa","aaaaaaa","aaaaaaaaaa","aaaaaaaaaaa","aaaaaaa"],
                2 : ["aaaaaaaa","aaaaaaa","aaaaaa","aaaaaaaa","aaaaaaaa","aaaaaaa","aaaaaaaaaa","aaaaaaaaaaa","aaaaaaa"],
                3 : ["aaaaaaaa","aaaaaaa","aaaaaa","aaaaaaaa","aaaaaaaa","aaaaaaa","aaaaaaaaaa","aaaaaaaaaaa","aaaaaaa"],
            }
        }
    }
}
</script>

<style scoped>
    #main-2-container {
        width : 100vw;
        background-image : url("C:/Users/anshm/Desktop/CFI project/New folder/FATHER_AGNEL_WEBSITE-CLONE/fasd-homepage/public/2.png");
        background-repeat : no-repeat ;
        background-size : cover;
        height : 100vh;
        display:flex;
        justify-content: center;
        align-items:center;
        align-content : center;

    }
    #scroller-1,#scroller-2,#scroller-3 {
        margin:15px;
        width: 25vw;
        height:70vh;
        background-color : rgba(255,255,255,0);


    }

    .heading {
        background-color: rgba(255,255,255, 0);
        font-size:30px;
        color:white;
        margin: 10px;
    }

    .scroller {
        width:100%;
        height:100%;
        border-style : solid;
        border-width:3px;
        border-color: red;
    }
</style>