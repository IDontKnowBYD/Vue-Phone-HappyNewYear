<template>
  <div id="app">
    <h1>{{word[0]}}</h1>
    <h1>{{word[1]}}</h1>
    <h1>{{word[2]}}</h1>
    <h1>{{word[3]}}</h1>
    <div v-if="surprise" class="imgContain">
    </div>
    
  </div>
</template>

<script>
export default {
  data () {
    return {
      surprise: false,
      word: ['祝','大','哥','']
    }
  },
  mounted: function() {
    setTimeout(() => {
      this.surprise = true;
      setTimeout(() => {
        this.surprise = false;
      }, 600);
    }, 13000);
    setTimeout(() => {
      this.word = ['新','年','快','乐'];
    }, 3000);
    setTimeout(() => {
      this.word = ['大','吉','大','利'];
    }, 6000);
    setTimeout(() => {
      this.word = ['早','生','贵','子'];
    }, 9000);
    setTimeout(() => {
      this.word = ['越','吃','越','胖'];
    }, 12000);
  },
  computed: {
    
  },
 
  methods: {
   
  }
}
</script>

<style>
  body {
    margin: 0;
    width: 100%;
    height: 100%;
    position: relative;
    background-color: red
  }
  #app {
    text-align: center;
    overflow: hidden;
  }
  #app h1 {
    font-size: 100px;
  }
  .imgContain {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 900px;
    background-image: url('./584533a00f2b6.jpg');
    background-position: center center;
    background-repeat: no-repeat;
  }
</style>
