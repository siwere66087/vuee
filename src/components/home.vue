


<template>
   <section class="home_container">

    <div class="card" v-for="item in personalDetails" :key="item">
   <!-- right content -->
<div class="right-content-container">
    <img :src="item.image" class="img">
<div class="card_body">
<h1 id="title">{{ item.title }}</h1>
<h1 id="titlle">{{ item.post }}</h1>

<div class="button" href="">for more info</div>
</div>
  
</div>
</div>
   </section>

<!-- <section class="left-content">
  <div class="card_left" v-for="item in leftContent" :key="item">




  </div>
</section> -->


</template>





<script>

export default {
 data() {
  return {
    // name:'card',
    personalDetails:[]
  }
 },
 mounted() {
  this.personalDetails = [{
  title:'siwe cele',
  post:'front-end-developer',
  image:'https://i.postimg.cc/9MfVKsb5/a.png'


  }]
//   this.leftContent = [{
//  greeting:'hi welcome to my page',
//  typetext: []


//   }]
 
 }
}
</script>



<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}



.home_container{
border: 3px solid green;
width: 100%;
height: 100vh;



}


.button{
width: 160px;
height: 40px;
margin-left: 45px;
background-color: yellowgreen;
}
/* .left-content{
width: 60%;
margin-top: 10px;
height: 70vh;
border: 5px solid rgb(216, 10, 10);
margin-right: 10rem;
float: right;


} */

.img{
width: 100%;
height: 190px;


}

.card{

border: 3px solid black;
width: 300px;
height: 400px;
margin-left: 10px;
position: relative;
background: linear-gradient(0deg, rgb(255, 24, 162), #2988e1);

}
.card::before, 
.card::after{
  content: '';
	position: absolute;
	left: -2px;
	top: -2px;
	background: linear-gradient(45deg, #fb0094, #0000ff, #00ff00,#ffff00, #ff0000, #fb0094, 
		#0000ff, #00ff00,#ffff00, #ff0000);
	/* background-size: 400%;
	width: calc(100% + 4px);
	height: calc(100% + 4px); */
	z-index: -1;
	animation: anime 20s linear infinite;
}

@keyframes anime {
	0% {
		background-position: 0 0;
	}
	50% {
		background-position: 400% 0;
	}
	100% {
		background-position: 0 0;
	}
}

.card:after {
	filter: blur(50px);
}




</style>
