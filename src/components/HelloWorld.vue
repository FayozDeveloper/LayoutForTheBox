<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      {{ title }}
      <a href="https://cli.vuejs.org" target="_blank" rel="noopener">vue-cli documentation</a>.
    </p>
    <ul v-for="todo in todosArray" :key="todo.id">
      <li>{{ todo.title }}</li>
    </ul>
    <h1>EcoTest</h1>
    <h1>Function in Function</h1>
    <test-component/>
  </div>
</template>

<script>
import TestComponent from "@/components/TestComponent";

export default {
  name: 'HelloWorld',
  components:{
    TestComponent,
  },
  props: {
    msg: String
  },
  data() {
    return {
      title: 'Something Test',
      search: "",
      todosArray: []
    }
  },
  methods: {
    fetchFunctionTest() {
      fetch("https://jsonplaceholder.typicode.com/todos")
          .then(response => response.json())
          .then(json => {
            this.todosArray = json;
            console.log(json)
          });
      // // axios.get('https://jsonplaceholder.typicode.com/todos')
      // // .then(res => (this.todosArray = res.data))
      // // .catch(error => console.log(error))
      //
      // this.axios.get('https://jsonplaceholder.typicode.com/todos').then((response) => {
      //   console.log(response.data)
      // })


    }
  },
  mounted() {
   this.fetchFunctionTest()

    // axios.get('www.thecocktaildb.com/api/json/v1/1/filter.php?c=Cocktail')
    // .then(res => (this.todosArray = res.data))
    // .catch(error => console.log(error))
  },
  // created() {
  //   this.fetchFunctionTest()
  // }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
