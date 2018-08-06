<template>
    <div>
      todolist
      <input type="text" v-model="inputVale">
      <button @click="addList">add</button>
      <ul>
        <li
          v-for="(item, index) in todolist"
          :key="index"
        >{{item}} <button @click="removeList(index)">remove</button></li>
      </ul>
    </div>
</template>

<script>
export default {
  name: 'todolist',
  data () {
    return {
      inputVale: '',
      todolist: [
        '1', '2', '3', '4', '5'
      ]
    }
  },
  methods: {
    addList: function () {
      if (this.inputVale !== '') {
        this.todolist.push(this.inputVale)
        this.inputVale = ''
      } else {
        alert('请输入内容')
      }
    },
    removeList: function (index) {
      console.log(index)
      this.todolist.splice(index, 1)
    }
  }
}
</script>

<style scoped>

</style>
