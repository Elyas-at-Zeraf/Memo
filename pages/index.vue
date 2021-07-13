<template>
  <div>
    <Form/>
  </div>
</template>

<script>
import Form from '../components/Form';

export default {
  layout: "home",
  components: {
    Form
    },
  data(){
    return {
      title: '',
      description: '',
    }
  },
  methods:{
    
  }
};
</script>
<style scoped>

</style>