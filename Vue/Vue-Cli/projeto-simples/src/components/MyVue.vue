<template>
  <div>
    <div id="cabecalho">{{ data }}</div>
    <div>
      <button id="btn" @click="add">aperte aqui para inserir um {{ message }}</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "MyVue",
  props: {
    msg: String
  },
  data: function() {
    return {
      data: "Esse é o meu trecho.",
      message: this.msg
    };
  },
  methods: {
    add() {
      this.data += " " + this.message;
    }
  }
};
</script>

<style scoped>
#cabecalho {
  background-color: aqua;
  width: 100%;
}
#btn{
  background-color: darkred;
  color:white;
}
</style>
