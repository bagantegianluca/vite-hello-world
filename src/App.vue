<script>
export default {
  name: 'App',
  data(){
    return{
      firstName: 'Gianluca',
      content: 'lorem ipsum color'
    }
  },
  methods:{
    functionLog(){
      console.log('Test');
      this.functionChild();
    },
    functionChild(){
      console.log('Child function');
    }
  }
}
</script>

<template>
  <div>
    <h1>Hello {{ firstName }}</h1>
    <p>{{ content }}</p>
    <button @click="functionLog">Click</button>
  </div>

</template>

<style>
</style>
