<template>
    <div>
    <form  @submit.prevent="submitHandler">
      <Title  />
      <Description />
      <Submit />
    </form>
    </div>
</template>

<script lang="ts">
    import Vue from 'vue'
    import Title from './Title.vue';
    import Description from './Description.vue';
    import Submit from './Submit.vue';

    export default Vue.extend({
       name: 'Form',
       components: {
        Title,
        Description,
        Submit,
        },
        methods:{
            submitHandler(){
             alert()
            }
        }
    })
</script>

<style scoped>
form{
  width: 80%;
  /* height: 100vh; */
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  
}
</style>