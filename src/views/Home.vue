<template>
  <div class="home">
    <app-header />
  </div>
</template>

<script>
// @ is an alias to /src
import {ref} from 'vue';
import AppHeader from '../components/app-header.vue';

export default {

  components: {
    AppHeader
  },
  setup(){

    const fname=ref('Abobakr');
    const lname=ref(' Rajab');
    const text=ref('app content');
    return {
      fname ,lname,text
    }
  }
  // data(){
  //   return{
  //   text:''
  //   }
  // }
};
</script>
<style >
  body{
    margin: 0px;
  }
</style>