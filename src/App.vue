<template>
  <div id="app">
    <my-cmp></my-cmp>
    <hr>
    <my-cmp></my-cmp>
  </div>
</template>

<script>
Vue.component('my-cmp', {
  data: function(){
    return {status: 'Critical'
    }
  },
  template: '<p>Server Status: {{ status }}</p>'
});

new Vue({
  el: '#app'
})
</script>

<style>
</style>
