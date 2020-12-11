<template>
  <div class="container">
    <template>{{a}}f</template>
    <div class="nested">
      <Module></Module>
      <router-link to="/page2">page2</router-link>
    </div>
    <button @click="testProxy">proxy data</button>
    <pre>{{proxyData}}</pre>
  </div>
</template>

<script>
import Module from './components/Module.vue';

export default {
  name: 'page',
  data() {
    return {
      a: 'page1',
      proxyData: {}
    };
  },
  components: {
    Module,
  },
  methods: {
    async testProxy() {
      let res = await axios.get('/api/Nosign/datavapi/teacher?token=XHX82NOT19NEED37LOGIN65&item_id=18&type=1')
      this.proxyData = res.data
    }
  }
};
</script>

<style scoped>
.container {
  color: red;
  .nested {
    font-size: 14px;
    color: var(--primary-color);
  }
}
</style>
