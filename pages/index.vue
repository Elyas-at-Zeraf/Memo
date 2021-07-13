<template>
  <div>
    <form  @submit.prevent="submitHandler">
      <div>
        <label for="">Title</label>
        <input type="text" v-model="title"/>
        <label >{{title}}</label>
      </div>
      <div>
        <label for="">Description</label>
      <textarea name="" id="" cols="30" rows="10" v-model="description"></textarea>
      </div>
      <div>
        <button type="submit">Submit</button>
      </div>
    </form>
  </div>
</template>

<script>
import Logo from "~/components/Logo.vue";
import VuetifyLogo from "~/components/VuetifyLogo.vue";
import home from "~/layouts/home";
export default {
  layout: "home",
  components: {},
  data(){
    return {
      title: '',
      description: '',
    }
  },
  methods:{
    submitHandler(){
      alert(this.title + this.description)
    }
  }
};
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
form div{
  display: flex;
  justify-content: start;
  align-items: center;
  
}
div input, div textarea{
  margin: 10px;
  border:1px solid black;
  border-radius: 13px;
}
button{
  border-radius: 13px;
  padding: 12px;
  background: #13131f;
  color: azure;
}
</style>