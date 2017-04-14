<template>
  <nav class="main-nav">
    <ul>
      <li v-for="item in links">
        <nuxt-link to={{ item.to }}>{{ item.text }}</nuxt-link>
      </li>
    </ul>
  </nav>
</template>

<script>
import Vue from 'vue';

export default Vue.component('vk-link-item', {
  props: [ 'links' ],
  data: () => ({
    links: []
  })
});
</script>

<style lang="scss" src="./navigation.scss"></style>
