<template>
  <div class="card-container">
    <div class="button-top-container">
      <a href=""><p>List</p></a>
      <p>Total:{{totalNum}}</p>
      <p>No.{{id}}</p>
    </div>
    <div class="content-container">
      <p class="content-text">{{ msg }}</p>
    </div>
    <div class="button-bottom-container">
      <button class="button-bottom button-bottom-rem">I remember</button>
      <button class="button-bottom button-bottom-check">Check</button>
      <button class="button-bottom button-bottom-norem">I don't remember</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'card',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      id: '123',
      totalNum: '578'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.card-container{
  border: 1px solid #999;
  border-radius: 10px; 
  width: 80%;
  margin: auto auto;
  position: relative;
  margin-top: 60px;
}
.button-top-container{
  display: flex;
  height: 50px;
  vertical-align: center;
  justify-content: space-between;
  width: 90%;
  border-bottom: 1px solid #eee;
  margin: 0 auto;
  align-items: center;
}

.content-container{
  min-height: 300px;
  display: flex;
}
.content-text{
  margin: auto auto;
  font-size: 18px;
  line-height: 18px;
  font-weight: 700;
}
.button-bottom-container{
  height: 50px;
  width: 90%;
  display: flex;
  left: 5%;
  justify-content: space-between;
  border-top: 1px solid #eee;
  margin: 0 auto;
}
.button-bottom{
  width: 90px;
}
</style>
