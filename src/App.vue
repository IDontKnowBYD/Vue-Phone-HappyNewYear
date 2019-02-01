<template>
  <div id="app">
    <h1>新</h1>
    <h1>年</h1>
    <h1>快</h1>
    <h1>乐</h1>
    <div class="imgContain">
    </div>
    
  </div>
</template>

<script>
export default {
  data () {
    return {
    }
  },
  computed: {
   
  },
 
  methods: {
   
  }
}
</script>

<style>
  body {
    width: 100%;
    height: 100%;
    position: relative;
    background-color: red
  }
  #app {
    text-align: center;
    background-color: red;
  }
  #app h1 {
    font-size: 100px;
  }
  .imgContain {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 800px;
    background-image: url('./584533a00f2b6.jpg');
    background-position: center center;
    background-repeat: no-repeat;
  }
</style>
