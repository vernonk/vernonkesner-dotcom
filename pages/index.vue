<template>
  <section>
    <hero/>
    <section class="columns">
      <vk-tile contentType="consulting"></vk-tile>
      <vk-tile contentType="development"></vk-tile>
    </section>
    <section class="columns">
      <vk-tile contentType="training"></vk-tile>
    </section>
  </section>
</template>

<script>
import Hero from '../components/Hero';
import Tile from '../components/Tile';

export default {
  components: {
    Hero,
    Tile
  }
};
</script>

<style lang="scss" src="./home.scss"></style>
