<template>
  <div id="app">
    
    <firstcom v-for="(count , j) in countries" :key ="j" :country="count.country" :capitalCity="count.capitalCity" :language="count.language"/>
  </div>
</template>

<script>
import firstcom from  './components/firstcom.vue'
import secondcom from  './components/secondcom.vue'

export default {
  name: 'app',
  data:function(){
    return{
      info:[ {
        name:"Faizan" ,
        fathername:"Zafar",
         CNIC:"12334"
      },
      {
        name:"Hassan" ,
        fathername:"Mushtaq",
        CNIC:"12334"
      },
      {
        name:"Arslan", 
        fathername:"Hanif",
        CNIC:"12334"
      },
      {
        name:"Adeel", 
        fathername:"hamza",
        CNIC:"12333244"
      }],
      countries: [
        {
          country: "Pakistan",
          capitalCity: "Islamabad",
          language: "Urdu"
        },
         {
          country: "China",
          capitalCity: "Beijing",
          language: "Chinese"
        },
         {
          country: "India",
          capitalCity: "Islamabad",
          language: "Urdu"
        },
         {
          country: "Pakistan",
          capitalCity: "Islamabad",
          language: "Urdu"
        },
         {
          country: "Pakistan",
          capitalCity: "Mumbai",
          language: "Hindi"
        },
         {
          country: "Afghanistan",
          capitalCity: "Kabul",
          language: "Afgani"
        }
      ]

    }
    
  },

  components: {
    firstcom,
    secondcom
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
