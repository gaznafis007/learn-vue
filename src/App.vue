<script>
export default {
  data() {
    return {
      name: 'Gazi Nafis Md Abdullah',
      status: true,
      tasks: ['task One', 'task Two', 'task Three'],
      link: 'https://gazi-nafis-rafi.vercel.app/',
    }
  },
  methods: {
    toggleStatus() {
      this.status = !this.status
    },
  },
}
</script>

<template>
  <h1>Hey, My name is {{ name }}</h1>
  <br />
  <p v-if="status">User is active</p>
  <p v-else>User is inactive</p>
  <a v-bind:href="link">visit my portfolio</a>
  <ul>
    <li v-for="task in tasks" :key="task">{{ task }}</li>
  </ul>

  <button @click="toggleStatus">change user status</button>
</template>
