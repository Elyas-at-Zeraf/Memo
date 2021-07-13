<template>
    <div>
        <label for="">Title</label>
        <input type="text" v-model="title"/>
        <label >{{title}}</label>
    </div>
</template>

<script lang="ts">
    import Vue from 'vue'

    export default Vue.extend({
        name: 'Title',
        data(){
            return{
                title: '',
            }  
        },
    })
</script>

<style scoped>
div{
  display: flex;
  justify-content: start;
  align-items: center;
  
}

input{
  margin: 10px;
  border:1px solid black;
  border-radius: 13px;
}
</style>