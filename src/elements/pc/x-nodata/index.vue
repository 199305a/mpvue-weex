<template>
  <div class="pc-x-nodata" element-path="pc/x-nodata">
  {{viewModel}}
  </div>
</template>

<script>
  export default {
    name: 'x-nodata',
    props: {
      elementData: {}
    },
    data () {
      return {
        viewModel: ''
      }
    },
    mounted () {
      this.init()
    },
    methods: {
      async init () {
        if (this.elementData !== undefined) {
          this.viewModel = this.elementData
        }
      }
    }
  }
</script>

<style lang="less">
  @import '~_style/index.less';
  .pc-x-nodata {
  	font-size: @font-size-base;
  }
</style>
