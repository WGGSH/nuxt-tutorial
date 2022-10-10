<template>
  <div>
    about me
    <button @click="action">
      show
    </button>
    <LazyTest v-if="show"></LazyTest>
  </div>
</template>

<script>
export default {
  data() {
    return {
      show: false
    }
  },
  methods: {
    action() {
      this.show = !this.show
    }
  }
}
</script>
