<template>
  <div class="container p-eyecatch">
    <logo class="p-eyecatch__logo" alt="murokacoの紹介ページ" />
    <a href="https://kacolog.netlify.app/" class="p-eyecatch__link">まだ何もないのでとりあえずブログを見に行く</a>
    <!-- <TheTheButton class="c-btn c-btn--primary">
      今まだ何もないのでとりあえずブログを見に行く
    </TheTheButton> -->
    <WipLabel />
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import WipLabel from '~/components/WipLabel.vue'
import TheButton from '~/components/TheButton.vue'

export default {
  head () {
    return {
      title: 'murokaco',
      meta: [
        { hid: 'description', name: 'description', content: 'My custom description'}
      ]
    }
  },
  components: {
    Logo,
    WipLabel,
    TheTheButton: TheButton,
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
.p-eyecatch {
  display: flex;
  flex-direction: column;
  &__logo {
    width: 340px;
  }
  &__link {
    display: inline-block;
    padding: 1rem 2rem;
    background: white;
    color: gray;
    font-weight: bold;
    text-decoration: none;
    border: 1px solid;
    border-radius: 50px;
    &:hover {
      background: gray;
      color: white;
    }
  }
}
</style>
