<template>
  <div class="hello">
    <div class="holder">
      <ul>
        <li v-for="(data, index) in skills" :key="index">
          {{ index }}. {{ data.skill }}
        </li>
      </ul>
      <div v-bind:style="{ backgroundColor: bgColor, width: bgWidth, height: bgHeight }">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Skills',
  data() {
    return {
      skills: [
      { "skill": "Vue.js" },
      { "skill": "React" },
      ],
      bgColor: '#eee',
      bgWidth: '100%',
      bgHeight: '30px'
    }
  }
}
</script>

<!-- "scoped" attribute limits CSS to this component only -->
<style scoped>
  ul {
    list-style: none;
  }
  .alert {
    background: #eee;
    width: 100%;
    height: 30px;
  }
  .another-class {
    border: 5px solid grey;
  }
</style>
