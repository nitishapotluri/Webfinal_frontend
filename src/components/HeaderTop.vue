<template>
    <div>
       <h1> {{Name}} </h1>
    </div>
</template>
    
    <script>
    
    export default{
        name: 'HeaderTop',
        props:{
            Name:String
  }
    }

</script>
    
<style scoped>
    
    div{
        text-align: center;
        color: black;
        
    }
    
</style>