<template>
  <div class="container">
    <logo class="p-top__logo" alt="murokacoの紹介ページ" />
    <WipLabel />
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import WipLabel from '~/components/WipLabel.vue'

export default {
  components: {
    Logo,
    WipLabel
  }
}
</script>

<style lang="scss">
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
