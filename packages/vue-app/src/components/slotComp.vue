<template>
  <div class="hello">
    <h1 @click="visible = !visible"> slot </h1>

    <div v-if="visible">
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SlotComp',
  data() {
    return {
      visible: false
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
