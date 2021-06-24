<template>
  <div class="hijo">
    <button class="btn btn-success" @click="number++">
      <span
        ><strong>{{ number }}</strong></span
      >
    </button>

  </div>
</template>
<script>
export default {

  data() {
    return {
      
      number: 0,
    };
  },
};
</script>

<style scoped>
.hijo {
  box-shadow: 0px 10px 10px -6px black;
  margin-top: 10px;
  margin-left: 10px;
  width: 200px;
}
button {
  color: #2c3e50;
  width: 200px;
  height: 50px;
  font-size: 18px;
  padding-left: 20px;
}

span {
  background: #2c3e50;
  color: #fff;
  font-size: 20px;
  padding: 10px;
  margin-left: 60px;
  cursor: pointer;
}
</style>