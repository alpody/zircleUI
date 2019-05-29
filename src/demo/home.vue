<template>
    <z-view style="border-width: 8px;">
        <div slot="label">
         WELCOME<br/>TO<br/>ZIRCLE UI
        </div>
    <div slot='extension'>
      <z-spot  
        :angle='45'
        to-view='docs'
        class='accent'
        >
        <div slot="label">
            docs<br/>docs
        </div>
        <i class='fas fa-book'></i>
      </z-spot>
      <z-spot
        button
        :angle='135'
        class='accent'
        label='Github'
        @click.native="openUrl">
        <i class='fab fa-github'></i>
      </z-spot>
    </div>
  </z-view>
</template>
<script>
export default {
  methods: {
    openUrl () {
      window.open('https://github.com/zircleUI/zircleUI', '_blank')
    }
  }
}
</script>
