<template>
  <div class="login-container">
    <!-- 卡片 -->
    <el-card class="login_box">
      <img src="../../assets/images/logo_index.png" alt="BG" />
      <!-- 表单 -->
      <el-form>
        <el-form-item>
          <el-input placeholder="请输入手机号"></el-input>
        </el-form-item>
        <el-form-item>
          <el-input placeholder="请输入验证码" class="text"></el-input>
          <el-button class="btn1">发送验证码</el-button>
        </el-form-item>
        <el-form-item>
          <el-checkbox v-model="checked"></el-checkbox>我已同意并同意
          <el-link type="primary">用户协议</el-link>和
          <el-link type="primary">隐私条款</el-link>
        </el-form-item>
        <el-form-item>
          <el-button class="btn2" type="primary">登录</el-button>
        </el-form-item>
      </el-form>
    </el-card>
  </div>
</template>

<script>
export default {
  data () {
    return {
      checked: true
    }
  }
}
</script>

<style scoped lang="less">
.login-container {
  width: 100%;
  height: 100%;
  position: absolute;
  left: 0;
  top: 0;
  background: url(../../assets/images/login_bg.jpg) no-repeat center / cover;
  .login_box {
    width: 450px;
    height: 350px;
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    img {
      display: block;
      width: 200px;
      margin: 10px auto 30px;
    }
  }
}
.el-checkbox {
  margin-right: 5px;
}
.text {
    width: 280px;
}
.btn1 {
    float: right
}
.btn2 {
    width: 100%
}
</style>
