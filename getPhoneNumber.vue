<template>
  <button hover-class="none" open-type="getAuthorize" scope="phoneNumber" @error="onError" @getAuthorize="onGetAuthorize">获取手机号</button>
</template>


<script lang="ts">
export default {
  
  data() {
    return {
      
    };
  },
  methods: {
    onError(e) {
      console.log('e: ', e)
    },
     onGetAuthorize() {
      console.log('onGetAuthorize res: ')
    },
  },
};
</script>
