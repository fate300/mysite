<template>
  <div class="container">
    <div class="item color1">item1 Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nisi necessitatibus fugiat qui labore, reprehenderit autem sequi aliquam ad beatae repellendus!</div>
    <div class="item color2">item2</div>
    <div class="item color3">item3</div>
    <div class="item color4">item4</div>
    <div class="item color5">item5</div>
    <div class="item color1">item6</div>
    <div class="item color2">item7</div>
    <div class="item color3">item8</div>
    <div class="item color4">item9</div>
    <div class="item color5">item10</div>




  </div>



</template>

<script>

export default {
  name: 'App',
  components: {
    
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
*  {
  box-sizing: border-box;
}

body {
  width: 100vw;
  height: 100vh;
  margin: 0;
}
.container {
display: grid;
grid-template-columns: repeat(5, 1fr);
/* colum을 설정하고 row는 auto 그리고 minmax를 이요하는 게 좋음  */
grid-auto-rows: minmax(150px,auto) ;
}

.item {
  display: flex;
  justify-content: center;
  align-items: center;
  border: 1px solid #181818;
  font-size: 1.2rem;
  font-weight: bold;
}

.color1 {
  background-color: #d7bee2;
}
.color2 {
  background-color: #a9c7d8;
}
.color3 {
  background-color: #c0df9f;
}
.color4 {
  background-color: #f2e5a6;
}
.color5 {
  background-color: #e89d9d;
}
</style>
