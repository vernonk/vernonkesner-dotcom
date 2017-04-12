<template>
  <section class="column">
    <template v-if="contentType === 'consulting'">
      <h2 class="title">{{ tileContent.consulting.title }}</h2>
      <p>{{tileContent.consulting.content}}</p>
    </template>
    <template v-else-if="contentType === 'development'">
      <h2 class="title">{{ tileContent.development.title }}</h2>
      <p>{{tileContent.development.content}}</p>
    </template>
    <template v-else-if="contentType === 'training'">
      <h2 class="title">{{ tileContent.training.title }}</h2>
      <p>{{tileContent.training.content}}</p>
    </template>
    <template v-else>
      <h2 class="title">{{ title }}</h2>
      <p class="content">{{content}}</p>
    </template>
  </section>
</template>

<script>
import Vue from 'vue';
import tileContent from './tile-content';

export default Vue.component('vk-tile', {
  props: [ 'title', 'content', 'contentType', 'className' ],
  data: () => ({
    tileContent
  })
});
</script>
