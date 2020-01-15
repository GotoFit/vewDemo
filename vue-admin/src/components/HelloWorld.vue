<template>
  <div class="hello">
    <h1>后台管理系统</h1>
    <el-form>
      <el-form-item>
        <el-input placeholder="请输入用户名" v-model="user" style="margin-bottom:1%">
          <i slot="prefix"  class="el-input__icon el-icon-search"></i>
        </el-input>
        <el-input placeholder="请输入密码" v-model="password">
          <i slot="prefix" class="el-input__icon el-icon-search" show-password></i>
        </el-input>
      </el-form-item>
      <el-form-item>
        <el-button type="primary" @click="onSubmit">登录</el-button>
        <el-button>取消</el-button>
      </el-form-item>
    </el-form>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      user: "",
      password: ""
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.el-input {
  /* width: 50%; */
}
</style>
