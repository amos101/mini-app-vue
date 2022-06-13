<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <div @click="btnChange()" id="btn">ルーレット</div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  methods: {
    btnChange() {
      const btn = document.getElementById("btn");
      btn.textContent = "hit";
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#btn {
  width: 200px;
  height: 200px;
  background: #ef454a;
  border-radius: 50%;
  margin: 30px auto;
  text-align: center;
  line-height: 200px;
  color: #fff;
  font-weight: bold;
  font-size: 22px;
  cursor: pointer;
  box-shadow: 0 10px 0 #d1483e;
  user-select: none;
}

#btn:hover {
  opacity: 0.9;
}

#btn:active {
  box-shadow: 0 5px 0 #d1483e;
  margin-top: 35px;
}
</style>
