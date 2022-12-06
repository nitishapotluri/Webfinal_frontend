<template>

    <div class ="box">
        <ul><h3 class = "item"> COLOR : {{Thrift.color}}</h3></ul>
        <ul><h3 class = "item"> BRAND : {{Thrift.Brand}}</h3></ul>
        <ul><h3 class = "item"> PRICE(USD) : {{Thrift.Price}}</h3></ul>
        <ul><h3 class = "item"> CONDITION : {{Thrift.Condition}}</h3></ul>
        <ul><h3 class = "item"> SIZE  :  {{Thrift.Size}}</h3></ul>
    </div>

</template>

<script>


export default{
    name: 'ThriftItem',
    props:{
        Thrift: Array
    }
}


</script>

<style scoped>


h4{
    margin: 2px;
}

div{
    background-color: skyblue;
    color: black;
    padding: 1em;
}
 

/*.item{
    font-size: 20px;
    font-family: 'Times New Roman', Times, serif;
    position: relative;
    flex-direction: column;
    min-width: 0;
    word-wrap: break-word;
    background-clip: border-box;
    border: 1px solid rgba(0,0,0,.125);
    border-radius: 0.25rem;
    color: white;
    background-color :rgb(13, 110, 253);
    margin-bottom: 1rem;
    width: calc(90% - 20px);
    display: flex; 
    padding: 0.5em
}*/

.box{
    background-color: #b8c8ed;
    color:rgb(2, 7, 16);
    padding: 1em;
    border:3px solid rgb(100, 146, 211);
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    width:100%;
    height:250px;
    word-wrap: break-word;
    font-size: 20px;
    position: relative;
}




</style>