<template>
  <div>
    <p>Holis</p>
  </div>
  <form>
    <input v-model="myName" class="input" type="text">
    <button class="btnSend" v-on:click="showName">Enviar</button>
    <p style="color: #000;">{{ myName }}</p>
  </form>

</template>

<script>
export default {
  name: 'HelloWorld',
  myName: null,
  props: {
    msg: String
  },
  methods: {
    showName: function(evt) {
      evt.preventDefault();
      alert("Hola");
    }
  }
}
</script>

<style>
.btnSend, .input {
  color: #000;
}
</style>
