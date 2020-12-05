<template>
  <div id="app">
    <header>
      
    </header>
    <div id="categories">
      <Category 
        v-for="cat in categories"
        v-bind:title="cat.name"
        v-bind:item="cat"
        v-bind:key="cat.id"
      ></Category>
    </div>
  </div>
</template>

<script>
import Category from './components/Category.vue'

export default {
  name: 'App',
  components: {
    Category
  },
  data: function() {
    return{
      categories: [
        {
          name: "Backlog",
          id:1,
          items: [
            {
              name: "TD1-1",
              description: "DESC1-1"
            },
            {
              name: "TD1-2",
              description: "DESC1-2"
            },
            {
              name: "TD1-3",
              description: "DESC1-3"
            }
          ]
        },
        {
          name: "Doing",
          id:2,
          items: [
          {
              name: "TD2-1",
              description: "DESC2-1"
            },
            {
              name: "TD2-2",
              description: "DESC2-2"
            },
            {
              name: "TD2-3",
              description: "DESC2-3"
            }
          ]
        },
        {
          name: "Done",
          id:3,
          items: [
          {
              name: "TD3-1",
              description: "DESC3-1"
            },
            {
              name: "TD3-2",
              description: "DESC3-2"
            },
            {
              name: "TD3-3",
              description: "DESC3-3"
            }
          ]
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
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
