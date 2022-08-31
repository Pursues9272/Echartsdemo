<template>
    <div class="index"><el-button type="primary">Primary</el-button></div>
  </template>

<script>
// @ is an alias to /src
export default {
  data () {
    return {}
  },
  mounted () {
    this.init()
  },
  methods: {
    async init () {
      const list = await this.axios.get('http://127.0.0.1:4523/m1/1278146-0-default/pet/2')
      console.log(list)
    }
  }
}
</script>

  <style lang="less" scoped>
  // 严格模式下必须存在内容
  </style>
