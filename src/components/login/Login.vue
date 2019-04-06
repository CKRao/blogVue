<template>
  <div class="login">
    <img src="../../assets/cklogo.png">
    <h3>{{ msg }}</h3>
    <div class="loginInput">
      <div class="inputcontainer">
       账号：
      <el-input v-model="account" type="input" placeholder="请输入账号" class="inputs"></el-input>
      </div>
      <div class="inputcontainer">
       密码：
      <el-input v-model="pwd" type="password" placeholder="请输入密码" class="inputs"></el-input>
      </div>
       <div class="buttoncontainer">
       <el-button type="primary" icon="el-icon-edit">注册</el-button>
      <el-button type="primary" icon="el-icon-menu">登录</el-button>
    </div>
    </div>

  </div>
</template>

<script>
export default {
    name: "login",
    data() {
      return {
        msg :'登录',
        account:'',
        pwd:''
      }
    }
}
</script>

<style>
body{
  text-align:center;
} 
  
.loginInput{
   margin:0 auto;
  /* text-align: center; */
  width: 30%
}

.inputs{
  float: right;
  width: 80%;
  height: 100%;
}

.inputcontainer{
  float: left;
  width: 100%;
  height: 50px;
  line-height:50px;
  margin-bottom: 1.5%;
}

.buttoncontainer{
  height: 40%;
  width: 100%;
  padding: 10px;
}

a {
  color: #ffffff;
  text-decoration: none;
}

.router-link-active {
  text-decoration: none;
}

</style>

