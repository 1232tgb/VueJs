<template>
  <div>
      <div id="image">
      <img src="../assets/logo.png" alt="imagem" />
    </div>
  </div>
</template>

<script>
export default {
  name: "MyOtherVue",
  data: function() {
    return {
      url: "../assets/logo.png"
    };
  },
  computed: {
    getSource() {
      return this.url;
    }
  }
};
</script>
<style lang="stylus" scoped></style>