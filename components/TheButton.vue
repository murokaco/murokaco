<template>
    <Button　:class="$attrs.class">
      <slot />
    </Button>
</template>
<style scoped lang="scss">
  Button {
    padding: 1rem 2rem;
    border: 1px solid black;
  }
</style>