<template>
  <div class="about">
    <h1>About Page</h1>
    <p>Hello {{ visitor_name }}!</p>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna ali...</p>
  </div>
</template>

<script>
export default {
  name: 'About',
  data() {
    return {
      visitor_name: this.$route.params.name
    }
  }
}
</script>
