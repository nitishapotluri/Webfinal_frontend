<template>
    <div class="Thriftbox">
        <div v-for="Thrift in Thrift" :key="Thrift.id" >
            <Item :Thrift="Thrift"/>
        </div>

    </div>
    


</template>'

<script>

    import Item from './Item.vue'


    export default{
        name: 'ThriftBox',
        components: {
            Item
        },
        props:{
            
            Thrift: Array
        }
    }

</script>

<style scoped>

.Thriftbox{

background-color: skyblue;
color: gray;
display: grid;
grid-template-columns: 1fr 1fr 1fr;
border:3px solid rgb(29, 70, 127)
}

</style>