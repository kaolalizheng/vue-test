<template>
  <div class="yangshi">
    <p>{{ a }}</p>
    <button @click="add">增加</button>
    <button @click="minus">减少</button>
    <button @click="division">除去</button>
    <p>{{ doubleA }}</p>
    <p>{{ squareA }}</p>
  </div>
</template>

<script>
  export default {
    data(){
      return {
        a:100
      }
    },
    created(){
      console.log('我是前端的新增');
    },
    methods:{
      add(){
        this.a++;
      },
      minus(){
        this.a--
      },
      division(){
        this.a=this.a/2;
      }
    },
    computed:{
      doubleA(){
        return this.a*2;
      },
      squareA(){
        return this.a*this.a;
      }
    }
  }
</script>

<style scoped>
.yangshi{
  background-color: aqua;
  font-size: 25px;
}
</style>