<template>
  <div class="hello">
    <span>{{msg}}</span>
    <div>
      {{money}} {{a}} {{b}}
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      money: 100,
      a: 10,
    }
  },
  computed: {
    b:function() {
      return this.money-this.a
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
