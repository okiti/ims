<template>
  <div class="flex nowrap col-lg-6">
    <defaultAside/>
    <div class="flex column nowrap col-lg-6 main-container">
      <defaultHeader/>
      <router-view></router-view>
    </div>
  </div>
</template>
<style lang="scss" scoped>
.main-container {
  margin: 0 50px;
  @media only screen and (max-width: 720px) {
    margin: 0;
  }
}
</style>
<script>
import defaultHeader from '@/components/header.vue';
import defaultAside from '@/components/sidebar.vue';

export default {
  components: {
    defaultHeader,
    defaultAside,
  },
};
</script>
