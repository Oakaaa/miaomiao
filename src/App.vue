<template>
  <div>
    <button>father button</button>
    <input type="text" v-model="mytext" />
    <HelloWorld myname="from father component">
      <div>slottest</div>
    </HelloWorld>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
// import Vue from 'vue'
// Vue.component('HelloWorld', HelloWorld)

export default {
  data() {
    return {
      mytext: '1256'
    }
  },
  components: {
    HelloWorld
  }
}
</script>

<!-- <script>
    export default{
        data(){
            return {
                mytext:"13254",
            }
        }
    }
</script> -->

<style lang="scss" scoped>
// #app{
//   font-family: Avenir, Helvetica, Arial, sans-serif;
//   -webkit-font-smoothing: antialiased;
//   -moz-osx-font-smoothing: grayscale;
//   text-align: center;
//   color: #2c3e50;
// }

// #nav {
//   padding: 30px;

//   a {
//     font-weight: bold;
//     color: #2c3e50;

//     &.router-link-exact-active {
//       color: #42b983;
//     }
//   }
// }
button{
  background-color: red;
}
</style>
