<template>
  <div class="container">
    <HeaderTop Name="My Thrift Store"  />

    <Box :Thrift="Thrift" />

</div>
</template>

<script>

import HeaderTop from './components/HeaderTop.vue'
import Box from './components/Box.vue'

export default {
  name: 'App',
  components: {    
    HeaderTop,
    Box
  },

  data(){
    return {
      Thrift: []
    }

  },

  methods: {

    // promises

      async fetchThrift(){
          //const res = await fetch('http://localhost:5959/Thrift')
          const res = await fetch('https://nitishanode.herokuapp.com/api')
          
          const data = await res.json()
          console.log( data )
          return data.Thrift
      }


  },
  async created(){
    this.Thrift = await this.fetchThrift()
  }
}

</script>

<style>

@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300&display=swap');
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: 'Montserrat', sans-serif;
}
.container {
  
  background-color: pink;
  margin: 30px auto;
  overflow: auto;
  min-height: 300px;
  border: 0.3em solid black;
  padding: 40px;
  border-radius: 5px;
  width:100%;;
}

div{
  margin-bottom: 0.5em;
  padding:10px;
}

</style>
