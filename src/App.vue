<template>
  <div class="yangshi">
    <p>{{ a }}</p>
    <button @click="add">增加</button>
  </div>
</template>

<script>
  export default {
    data(){
      return {
        a:100
      }
    },
    methods:{
      add(){
        this.a++;
      },
    }
  }
</script>

<style scoped>
.yangshi{
  background-color: red;
}
p{
  background-color: aqua;
  font-size: 20px;
}
</style>
