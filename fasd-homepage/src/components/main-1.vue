<template>

    <article id="main-one">
        <div id="m1-header"> 
          <div id="m1-toolbox" >
            <div class="m1-tools" v-for="tools1 in toolbox1" :key="tools1"> {{tools1}}</div>
          </div>
          <div style=" position : relative; height:90vh; width:100vw;">
            <div style="position : absolute;">
              <div id="main-one-images" >
                <img v-for="(source,index) in sources" :key="source" class="m1-image" :id = get_id_m1(index)  :src=form_img_src_m1(index)  width="100" height="20">
              </div>
            </div>
            <div style=" position :absolute; width:3vw; height:90vh; right:0px; " >
              <button  class="m-one-button"  v-for="(source,index) in sources" :key="source" :id=form_m1_id(index)  @click="slider=index;  slider_main(); " > {{index}} </button>
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
    name : "mainOne",
    data () {
        return {
            toolbox1 : ["What WE ARE" , "STUDENT'S HUB" , "ADMIN" , "CAMPUS BUZZ" , "BUS ROUTES AND ACCESS" , "OUTREACH" ,"FAA (ALUMINI)","CAMPUSCARE"],
            sources : ["1.png" ,"2.png","3.png","4.png","5.png" ],
            slider : 0,
        }
    },
    methods : {
    get_id_m1 (index) {
      var a = "m";
      a+=index;
      a+="-image"
      return a
    },
    form_img_src_m1(index) {
      var a = this.sources[index]
      return a
    },
    form_m1_id (index) {
      var a= "m";
      ++index;
      a+=index;
      a+="-button"
      return a
    },
    slider_main () {
        console.log(this.slider)
        for (var i=0 ; i< this.sources.length ; ++i) {
          var a = document.getElementById( 'm' + i + '-image' )
          if (i!==this.slider) a.style.display="none"
          else a.style.display = "block"

        }
    } 
  },
}

</script>

<style scoped>
.m-one-button {
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
  .m1-image {
    position :absolute;
    width:100%;
    height:100%;
  }
  
  #maintext {
    color :navy;
    padding : 20px;
    margin : 10px;
  }
  
  #main-one {
    display : flex;
    align-items: center;
    padding-top : 10px;
    padding-bottom : 20px;
    margin-top : 10px;
    margin-bottom : 20px;
  
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
    margin-bottom : 40px;
  }
  
</style>