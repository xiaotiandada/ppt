<template>
  <div class="hello">
    todolist

    <p :class="{active: isActive}" v-on:click="eventsClicks" v-bind:title="msg">{{msg}}</p>

    <input type="text" v-model="one">
    <p>{{one}}</p>
    <p>{{calculation}}</p>

    <p v-if="isActive">true</p>
    <p v-else>false</p>

    <p v-show="isActive">show</p>

    <hr>

    <ul>
      <li v-for="(item, index) in items" :key="index">{{item.message}}</li>
    </ul>

    <child></child>
  </div>
</template>

<script>
import child from './child'
export default {
  name: 'HelloWorld',
  components: {
    child
  },
  data () {
    return {
      msg: 'I"m boornet',
      one: '',
      isActive: true,
      items: [
        {
          message: 'one'
        },
        {
          message: 'one'
        },
        {
          message: 'one'
        }
      ]
    }
  },
  methods: {
    eventsClicks: function () {
      this.isActive = !this.isActive
    }
  },
  computed: {
    calculation: function () {
      return this.msg.split('').reverse().join('')
    }
  },
  watch: {
    calculation: function () {
      console.log(this.calculation)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
