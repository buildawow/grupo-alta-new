<template>
  <div class="image-header" :style="{background: `url(${ require(`@/assets/${background}`) })`, backgroundPosition: backgroundPosition, backgroundSize: 'cover', backgroundRepeat: 'no-repeat' }">

  </div>
</template>

<script>
export default {
    name: 'ImageHeader',
    props: {
        background: String,
        backgroundPosition: String
    }
}
</script>

<style lang="scss" scoped>
    .image-header {
        height: 600px;
        @include tablet {
            height: 300px;
        }
        width: 100%;
    }
</style>