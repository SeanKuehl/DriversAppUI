<template>
  <button @click="toggle">Toggle</button>
  <div v-if="active">
    <h1>hello</h1>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        active: false,
        showTitle: ""
      }
    },
    methods: {
      toggle () {
        this.active = !this.active
        
      }
    },
    props: {
    options: Array,
    title: String,
    
  }
  }
</script>
