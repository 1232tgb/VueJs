<template>
  <div class="contador">
    <input type="number" v-model="valorCalculo" />

    <p>
      valor de calculo:
      <b>{{valorCalculo}}</b>
    </p>

    <span>{{ contador }}</span>
    <button @click="soma()">+</button>
    <button @click="subtrai()">-</button>
  </div>
</template>

<script>
export default {
  name: "contador",
  data: function() {
    return {
      contador: 0,
      valorCalculo: 0
    };
  },
  methods: {
    soma() {
      this.contador += Number.parseInt(this.valorCalculo);
    },
    subtrai() {
      this.contador -= this.valorCalculo;
    }
  }
};
</script>]

<style>
.contador span {
  border-bottom: 1px solid #ccc;
  height: 30px;
  padding: 5px 25px;
}
.contador button {
  height: 30px;
  width: 30px;
  border-radius: 15px;
  background-color: coral;
  color: #fff;
  margin-left: 10px;
  outline: none;
}
</style>>