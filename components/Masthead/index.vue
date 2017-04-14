<template>
  <div class="masthead">
    <div class="columns">
      <div class="column is-two-thirds">
        <a class="title" href="/">Vernon Kesner</a>
      </div>
      <div class="column">
        Front End Consulting, Development, and Training
      </div>
    </div>
    <navigation :links=navLinks />
  </div>
</template>

<script>
import Navigation from '../Navigation';

const navLinks = [
  {
    to: '/consulting',
    text: 'Consulting'
  },
  {
    to: '/development',
    text: 'Development'
  },
  {
    to: '/training',
    text: 'Training'
  },
  {
    to: '/speaking',
    text: 'Speaking'
  },
  {
    to: '/about',
    text: 'About'
  },
  {
    to: '/blog',
    text: 'Blog'
  },
  {
    to: '/contact',
    text: 'Contact'
  }
];

export default {
  components: {
    Navigation
  },
  data: () => ({
    navLinks
  })
};
</script>
<style src="./masthead.scss"></style>
