<template>
  <div class="hello">
    <img src="../assets/cklogo.png">
    <h1>{{ msg }}</h1>
    <div class="hello-button">
      <el-button type="primary" icon="el-icon-info" @click="aboutMe">关于</el-button>
      <el-button type="primary" icon="el-icon-menu"><router-link  to="/login">登录</router-link></el-button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  methods: {
     aboutMe:function() {
      const h = this.$createElement;
      this.$message({
         message: h('p', null, [
            h('span', null, '这是'),
            h('i', { style: 'color: teal' }, 'ClarkRaoHub')
          ])
      });
    }
  },
  data () {
    return {
      msg: 'Welcome to ClarkRao\'s Hub '
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
a {
  color: #ffffff;
  text-decoration: none;
}
.router-link-active {
  text-decoration: none;
}
</style>
