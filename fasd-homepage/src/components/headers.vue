<template>
    <div id="header-top">
        <div id="toolbox" >
          <div class="tools" v-for="tools in toolbox" :key="tools"> <img class="toolbox-img" src="logo.png"> {{tools}}</div>
         </div>
      </div>
    
    
      <div id="headerbottom">
          <div id="hb-wrapper">
            <img id="hb-img" src="logo.png">
            <h1 id="maintext">FATHER AGNEL SCHOOL, NEW DELHI</h1>
            <img id="hb-img" src="logo.png">
    
          </div>
      </div>
</template>

<script>
    export default {
        name:"headersTop",
        data () {
            return {
            toolbox : ["Google Map" , "Contact Us" , "Alerts" , "Mandatory Public Disclosure" , "Login"],
            }
        },
    }
</script>

<style scoped>
#header-top {
    display : grid;
    justify-content: space-around;
    align-items: center;
  }
  #toolbox {
    display : flex;
    width : 46vw;
    justify-content:space-around;
  
  }
  .toolbox-img {
    height: 15px;
    align-self: center;
  }
  .tools {
    display : inline-block;
    align-items: center;
    align-content: center;
    border : 5px;
    padding: 10px;
    padding-top: 0px;
    color : white;
    background-color:crimson;
    border-radius: 3px;
  }
  #headerbottom {
    display : flex;
    align-items: center;
    justify-content: center;
  
  }
  #hb-wrapper {
    display : flex;
    align-items: center;
    font-size : 20px;
    width:100vw;
  }

  #hb-img {
    width : 20vw;
    padding : 20px;
    margin : 10px;
    padding-left: 0%;
    padding-right: 0%;
    margin-left: 0%;
    margin-right: 0%;
    height: 20vh;
  }

</style>