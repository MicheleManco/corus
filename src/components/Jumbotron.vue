<template>
  <div class="big-container">
    <div class="container">
      <div class="row">
        <div class="col-9 row debug1">
          1 <br>
          1
          <div class="col-12 debug3 d-flex justify-content-end">
            1.1 <br>
            sdagbvjsaoighdgikodeng
          </div>
        </div>
        <div class="col-3 debug2">
          2
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'jumbotron',
  props: {
   
  }
}
</script>

<style scoped lang="scss">
.big-container{
  background-image: url("../assets/jumbotron.jpg");
  height: 800px;
  background-repeat: no-repeat;
  background-size: 100%;
}

.debug1{
  background-color: red;
}
.debug2{
  background-color: pink;
}

.debug3{
  background-color: purple;
}
</style>
