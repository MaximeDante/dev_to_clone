<template>
  <footer>
    <span>Build with</span>
    <a href="https://nuxtjs.org" target="_blank">
      <nuxt-icon class="nuxt-icon" />
    </a>
    <span>&</span>
    <a href="https://docs.dev.to/api" rel="nofollow noopener" target="_blank">
      <dev-to-icon />
    </a>
    <span>&</span>
    <span> By Maxime 🚀</span>
  </footer>
</template>

<script>
import DevToIcon from '@/assets/icons/dev-to.svg?inline'
import NuxtIcon from '@/assets/icons/nuxt.svg?inline'
export default {
  components: {
    DevToIcon,
    NuxtIcon
  }
}
</script>

<style lang="scss" scoped>
footer {
  padding: 2rem;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
  span {
    display: inline-block;
    line-height: 1;
    text-transform: uppercase;
    letter-spacing: $-ls2;
    font-size: $text-xs;
    font-weight: $bold-body-font-weight;
  }
  span:last-child{
    margin-left: 0.5rem;
    text-transform: capitalize;
  }
  a {
    svg {
      width: 3rem;
      height: 3rem;
      margin: 0 0.5rem;
    }
    .nuxt-icon {
      width: 2.5rem;
      height: 2.5rem;
      margin: 0 0.25rem;
    }
  }
}
</style>
