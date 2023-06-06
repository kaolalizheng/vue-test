<template>
  <div class="yangshi">
    <p>{{ a }}</p>
    <button @click="add">增加</button>
    <button @click="minus">减少</button>
    <button @click="division">除去</button>
    <p>{{ doubleA }}</p>
    <p>{{ squareA }}</p>
    <p>********************</p>
    <p>{{ b }}</p>
    <button @click="change">改变</button>
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
      },
      change(){
        this.b='刘德华'
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
p{
  background: red;
  font-weight: bold;
  color: aqua;
}
</style>