<template>
  <input :class="[searchFixed ? 'class-fixed' : '']" />
</template>

<style>
.class-fixed {
  position: fixed;
  top: 0;
}
</style>

<script lang="ts">
export default {
  props: {
    searchFixed: {
      type: Boolean
    }
  },
  
  data() {
    return {
      
    };
  },
  methods: {
  
  },
};
</script>
