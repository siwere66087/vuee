<template>
<h1></h1>
    <div class="home_container" >

       
    <personalDetails></personalDetails>
    </div>
</template>

<script>
// @ is an alias to /src
import personalDetails from '../components/home.vue'
// import leftContent from '../components/home.vue'

export default {
  name: 'card',
  components: {personalDetails}
}
</script>


