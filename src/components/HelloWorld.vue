<template>
  <div class="hello">
    <img src="../assets/cklogo.png">
    <h1>{{ msg }}</h1>
    <div class="hello-button">
      <el-button type="primary" icon="el-icon-info" @click="aboutMe">关于</el-button>
      <router-link  to="/login"><el-button type="primary" icon="el-icon-menu">登录</el-button></router-link>
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

.hello {
  display: flex;
  justify-content: center; /* 水平居中 */
  align-items: center;     /* 垂直居中 */
  width: 100%;
  height: 100%;
  flex-direction:column;
}
</style>
