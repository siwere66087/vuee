<template>
    

    <div class="carousel">
        <div id="carouselExampleControls" class="carousel slide" data-bs-ride="carousel">
            <div class="carousel-inner">
              <div class="carousel-item active">
                <div class="card" v-for="item in cards" :key="item">
                    <img src="item.image" >
                    <div class="card-body">
                      <h5 class="card-title">Life Choices Student</h5>
                      <i class="fa fa-quotes"></i>
                       <p class="card-text fst-italic"> Nontobeko  is a humble person who also takes pride in her work and makes sure she gets it done on time.She makes sure that everyone working with her has everything they need to make the job gets done eficiently and on time.</p>
                       <p>-Sivuyisiwe Mgijima</p>
                    </div>
                  </div>
              </div>
              
             
              
              </div>
            </div>
            <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
              <span class="carousel-control-prev-icon" aria-hidden="true"></span>
              <span class="visually-hidden">Previous</span>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
              <span class="carousel-control-next-icon" aria-hidden="true"></span>
              <span class="visually-hidden">Next</span>
            </button>
          </div>
      



</template> 

 <script>


    export default {
        data () {
    return {
      cards: [],
     
    }
  },
  mounted () {
    this.cards = [{
        
        name:"aliya",
        description:"siwe is a great person. she listes and very easy to talk to. shes's also hard working. ",
        image:"https://i.postimg.cc/mrpFBfKN/aliya.jpg",
        socialIcon:[]
        
    },

    {
        name:"Nontobeko Mhlongo",
        description:"siwe is a hard worker and easy person to be friend's with. she is also very helpful ",
        image:"https://i.postimg.cc/m23H1mmv/nonto.jpg",
        socialIcon:[]
    
    
    
     },

      {
        name:"aliya",
        description:" siwe is a hard worker and easy person to be friend's with. she is also very helpful",
        image:"https://i.postimg.cc/mrpFBfKN/aliya.jpg",
        socialIcon:[]
    
    },
     {
        name:"aliya",
        description:"siwe is a hard worker and easy person to be friend's with. she is also very helpful ",
        image:"https://i.postimg.cc/mrpFBfKN/aliya.jpg",
        socialIcon:[]
    
    
    },
    {
        name:"aliya",
        description:"siwe is a hard worker and easy person to be friend's with. she is also very helpful ",
        image:"https://i.postimg.cc/mrpFBfKN/aliya.jpg",
        socialIcon:[]
    
    
    }
    ]
   
  }
}

</script>

<style  scoped>

.carousel{
    background-color: yellow;
}



.img{
width: 100px;
height: 120px;

}
#testamonials{

background-color: yellow;


}
/* optional */
button {
  margin-right: 5px;
  margin-top: 10px;
}
</style> 



















