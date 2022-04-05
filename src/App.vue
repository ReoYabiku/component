<template>
  <div>
    <header class="header-logo">
      Component
    </header>
    <div class="boxes">
      <NameAndAge v-for="item in items" v-bind:key="item.id" v-bind:name="item.name" v-bind:age="item.age"></NameAndAge>
    </div>
    <footer class="footer-logo">
      fever time 6th
    </footer>
    <hr width=95% align="right">
  </div>
  
</template>

<script>
import NameAndAge from './components/NameAndAge.vue'

export default {
  name: 'App',
  components: {
    NameAndAge
  },
  data () {
    return{
      items:[
        {
          id: 1,
          name: "aaa",
          age: 123
        },
        {
          id: 2,
          name: "bbb",
          age: 45
        },
        {
          id: 3,
          name: "ccc",
          age: 78
        }
      ]
    }
}
}


</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

.header-logo{
  font-size: 50px;
  color: #999;
  font-weight: bold;
}

.footer-logo{
  font-size: 20px;
  color: black;
  text-align: right;
  padding: 0 20px;
  margin-bottom: -8px;
}

.boxes{
  display: flex;
  text-align: center;
  justify-content: center;
}

hr{
  text-align: right;
  margin-right: 0;
  margin-bottom: 40px;
}
</style>
