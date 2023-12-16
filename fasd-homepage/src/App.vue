<template>
  <div id="header-top">
    <div id="toolbox" >
      <div class="tools" v-for="tools in toolbox" :key="tools"> <img class="toolbox-img" src="fasd-homepage\src\assets\logo.png"> {{tools}}</div>
     </div>
  </div>


  <div id="headerbottom">
      <div id="hb-wrapper">
        <img id="hb-img" src="fasd-homepage\src\assets\logo.png">
        <h1 id="maintext">FATHER AGNEL SCHOOL, NEW DELHI</h1>
        <img id="hb-img" src="fasd-homepage\src\assets\logo.png">
      </div>
  </div>

  <div id="main-one">
    <div id="m1-header"> 
      <div id="m1-toolbox" >
        <div class="m1-tools" v-for="tools1 in toolbox1" :key="tools1"> {{tools1}}</div>
       </div>
    </div>
    <div id="main-one-images">
        <img src="fasd-homepage\src\assets\logo.png">
        <div>slideshow need to be here</div>
    </div>
  </div>

</template>

<script>
export default {
  name : "App" ,
  data () {
    return {
      toolbox : ["Google Map" , "Contact Us" , "Alerts" , "Mandatory Public Disclosure" , "Login"],
      toolbox1 : ["What WE ARE" , "STUDENT'S HUB" , "ADMIN" , "CAMPUS BUZZ" , "BUS ROUTES AND ACCESS" , "OUTREACH" ,"FAA (ALUMINI)","CAMPUSCARE"]
    }
  }
}

</script>

<style>
#header-top {
  display : grid;
  justify-content: space-around;
  align-items: center;
}
#toolbox {
  display : flex;
  width : 40vw;
  justify-content:space-around;

}
.toolbox-img {
  height: 10px;
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
}
#maintext {
  color :navy;
  padding : 20px;
  margin : 10px;
}
#hb-img {
  padding : 20px;
  margin : 10px;
  height: 15vh;
}
#main-one {
  display : flex;
  align-items: center;
}
#m1-header {
  width :100vw;
  border-width: 10px;
  border-style: solid ;
  border-color: yellow;
}
#m1-toolbox {
  display : flex;
  width : 100vw;
  align-items: center;
  justify-content :space-around;
  padding :5px;
  background-color : rgb(39, 39, 202);
}

.m1-tools {
  display : inline-block;
  align-items: center;
  align-content: center;
  text-align: middle;
  vertical-align: middle;
  padding: 5px;
  color : white;
  border-radius: 3px;
}
#main-one-images {
  border-width: 10px;
  border-style: solid;
  border-color: yellow;
}
</style>