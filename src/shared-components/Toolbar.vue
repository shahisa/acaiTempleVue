<template lang="html">
  <md-toolbar>
    <!-- <md-button class="md-icon-button"
      v-show="!hideMenu"
      @click="toggleSidenav">
      <md-icon>menu</md-icon>
    </md-button> -->

    <h2 class="md-title"
      style="flex: 1">
      {{ title }}
    </h2>

    <md-button class="md-button"
      v-for="option in options">
      <span v-text="option.text"></span>
    </md-button>

  </md-toolbar>
</template>

<script type="text/javascript">
  export default {
    props: {
      hideMenu: {
        type: Boolean,
        default() { return false; },
      },
      title: {
        type: String,
        default() { return ''; },
      },
      options: {
        type: Array,
        default() { return [
          { text: 'beta' },
          { text: 'blog' },
        ]; },
      },
    },
    data() {
      return {
        progress: 0,
        progressInterval: null,
        done: false,
        transition: true,
      };
    },
    components: {
    },
    methods: {
      toggleSidenav() {
        this.$emit('TOGGLE_SIDEBAR');
      },
    },
  };
</script>

<style media="screen">

</style>
