<template>
  <searchInput :searchFixed="searchFixed"></searchInput>
</template>


<script lang="ts">
import searchInput from './searchInput.vue'
export default {
  components: {
    searchInput
  },
  
  data() {
    return {
      searchFixed: false
    };
  },
  onPageScroll(e){
    if (e.scrollTop > 300 ) {
      this.searchFixed = true
    }
  },
  methods: {
  
  },
};
</script>
