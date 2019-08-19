
<template>

<el-container>
  <el-aside width="20%">Aside</el-aside>
  <el-container>
    <el-header>Header</el-header>
    <el-main>Main</el-main>
    <el-footer>Footer</el-footer>
  </el-container>
</el-container>

</template>

<script>
export default {
  name: 'backstageIndex',
  methods: {
  },
  data () {
    return {
      msg: 'Welcome to ClarkRao\'s Hub '
    }
  }
}
</script>
<style>
  .el-header, .el-footer {
    background-color: #B3C0D1;
    color: #75adff;
    text-align: center;
    line-height: 60px;
  }

  .el-main {
    text-align: center;
  }

  .el-aside {
    background-color: #D3DCE6;
    color: #75adff;
    text-align: center;
    line-height: 500px;
  }
</style>