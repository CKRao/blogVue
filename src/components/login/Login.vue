<template>
  <div class="login">
    <img src="../../assets/cklogo.png">
    <h3>{{ msg }}</h3>
    <div class="loginInput">
      <div class="inputcontainer">
       <label> 账号：</label>
       <el-input v-model="account" type="input" placeholder="请输入账号" class="inputs"></el-input>
      </div>
      <div class="inputcontainer">
       <label>密码：</label>
       <el-input v-model="pwd" type="password" placeholder="请输入密码" class="inputs"></el-input>
      </div>
       <div class="buttoncontainer">
      <el-button type="primary" icon="el-icon-edit">注册</el-button>
      <el-button type="primary" icon="el-icon-menu" @click="login">登录</el-button>
    </div>
    </div>

  </div>
</template>

<script>
export default {
    name: "login",
    methods : { 
      login:function(){
        this.$router.push('/backstageIndex')
      }
    },
    data() {
      return {
        msg :'登录',
        account:'',
        pwd:''
      }
    }
}
</script>

<style scoped>
body{
  display: flex;
  justify-content: center; /* 水平居中 */
  align-items: center;     /* 垂直居中 */
  width: 100%;
  height: 100%;
  flex-direction:column;
} 

  
.loginInput{
  margin:0 auto;
  width: 30%
}

.inputs{
  width: 80%;
  height: 100%;
  justify-content: center; /* 水平居中 */
  align-items: center;     /* 垂直居中 */
  flex-direction:column;
}

.inputcontainer{
  justify-content: center; /* 水平居中 */
  align-items: center;     /* 垂直居中 */
  flex-direction:row;
  width: 100%;
  height: 50px;
  line-height:50px;
  margin-bottom: 1.5%;
  flex-flow:wrap;
}

.buttoncontainer{
  height: 40%;
  width: 100%;
  padding: 10px;
  display: flex;
  justify-content: center; /* 水平居中 */
  align-items: center;     /* 垂直居中 */
  flex-direction:row;
}

a {
  color: #ffffff;
  text-decoration: none;
}

.router-link-active {
  text-decoration: none;
}

</style>

