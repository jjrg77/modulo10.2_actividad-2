<template>
  <div class="padre">
    <div class="titlePadre">
      <p>
        <strong>{{ message }}</strong>
      </p>
      <div class="divHijo" v-for="item in items" :key="item">
        hijo {{ item }}
        <Hijo></Hijo>
      </div>
    </div>
  </div>
</template>
<script>
import Hijo from "@/components/Hijo.vue";
export default {
  data() {
    return {
      message: "componente padre",
      items: [1, 2, 3],
    };
  },
  components: {
    Hijo,
  },
};
</script>

<style scoped>
.padre {
  padding: 50px;
  border: 1px solid #2c3e50;
  box-shadow: 0px 10px 10px -6px black;
  color: #fff;
  background: #27ae60;
  width: 70vw;
  height: 15rem;
  margin: 4vh auto;
}
.titlePadre {
  text-decoration: underline #fff;
}
.hijo {
  display: flex;
  justify-content: space-around;
}
.divHijo {
  float: left;
  justify-content: center;
  margin-top: 4vh;
  margin-left: 6vw;
}
</style>