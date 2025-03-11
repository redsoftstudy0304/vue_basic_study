!<template>
  <app-header v-bind:propsdata="str" v-on:renew="renewStr"></app-header>
</template>

<script>
import AppHeader from './components/AppHeader.vue';
export default {
  data: function(){
    return{
      str : 'xxxx'
    }
  },
  components :{
    'app-header':AppHeader,
  },
  methods:{
    renewStr:function(str) {
      this.str = str
    }
  }
}
</script>

<style>

</style>