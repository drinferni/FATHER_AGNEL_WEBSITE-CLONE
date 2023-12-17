<template>
  <div id="header-top">
    <div id="toolbox" >
      <div class="tools" v-for="tools in toolbox" :key="tools"> <img class="toolbox-img" src="./assets/logo.png"> {{tools}}</div>
     </div>
  </div>


  <div id="headerbottom">
      <div id="hb-wrapper">
        <img id="hb-img" src="./assets/logo.png">
        <h1 id="maintext">FATHER AGNEL SCHOOL, NEW DELHI</h1>
        <img id="hb-img" src="./assets/logo.png">

      </div>
  </div>

  <article id="main-one">
    <div id="m1-header"> 
      <div id="m1-toolbox" >
        <div class="m1-tools" v-for="tools1 in toolbox1" :key="tools1"> {{tools1}}</div>
      </div>
      <div style=" position : relative; height:90vh; width:100vw;">
        <div style="position : absolute;">
          <div id="main-one-images" >
            <img v-for="source in sources" :key="source" id="m1-image" src="./assets/logo.png"  width="100" height="20">
          </div>
        </div>
        <div style=" position :absolute; width:3vw; height:90vh; right:0px; ">
          <button id="m1-button"  v-for="(source,index) in sources" :key="source"> {{index}}</button>
        </div>
      </div>
    </div>
  </article>
  <article style="display:flex; justify-content:center;">
    <div id="main-two" >
            <span><center><h1 style="font-size : 30px;">Welcome to Fr. Agnel School</h1></center></span>
<span><center>
  FR. AGNEL SENIOR SECONDARY SCHOOL, GAUTAM NAGAR was established in 1979. 
  The school is affiliated to the C.B.S.E and seeks to nurture the talents of each student in a conducive environment. 
  The school endeavours to contribute towards the holistic development of each individual. Special emphasis is laid on 
  character building and on national integration.<br><br>
  The school is also a center of The National Open School which conducts classes for the differently abled in the school premises. 
  In addition the School also runs an urban slum community centre where about 400 students (children and adults) are educated and skill 
  trained.
</center></span>
</div>
  </article>
</template>

<script>
export default {
  name : "App" ,
  data () {
    return {
      toolbox : ["Google Map" , "Contact Us" , "Alerts" , "Mandatory Public Disclosure" , "Login"],
      toolbox1 : ["What WE ARE" , "STUDENT'S HUB" , "ADMIN" , "CAMPUS BUZZ" , "BUS ROUTES AND ACCESS" , "OUTREACH" ,"FAA (ALUMINI)","CAMPUSCARE"],
      sources : ["logo.png" ,"logo.png","logo.png","logo.png","logo.png" ]
    }
  }
}

</script>

<style>
#m1-button {
  display : block;
  position :relative;
  right : 0px;
  top : 40%;
  z-index: 10;
}
#main-one-images {
  position : relative;
  height : 90vh;
}
#m1-image {
  position :absolute;
  width:100%;
  height:100%;
}
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
}
#maintext {
  color :navy;
  padding : 20px;
  margin : 10px;
}
#hb-img {
  padding : 20px;
  margin : 10px;
  height: 20vh;
}
#main-one {
  display : flex;
  align-items: center;
  padding-top : 10px;
  padding-bottom : 10px;
  margin-top : 10px;
  margin-bottom : 10px;

}
#m1-header {
  width :100vw;
}
#m1-toolbox {
  display : flex;
  width : 100vw;
  align-items: center;
  justify-content :space-around;
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
  width : 100vw;
}

#main-two {
  display : grid;
  align-items: center;
  align-content: center;
  width: 60%;
}

</style>