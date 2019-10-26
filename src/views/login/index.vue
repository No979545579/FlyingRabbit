<template>
  <div class="container bgc">
    <el-card class="box-card">
      <img src="../../assets/logo_index.png" alt />
      <el-form>
        <el-form-item>
          <el-input placeholder="请输入手机号"></el-input>
        </el-form-item>
        <el-form-item>
          <el-input placeholder="请输入验证码" style="width:72%"></el-input>
          <el-button style="margin-left:10px">发送验证码</el-button>
        </el-form-item>
        <el-form-item>
          <el-checkbox label="我已阅读并同意用户协议和隐私条款" name="type" :value="true"></el-checkbox>
        </el-form-item>
        <el-form-item>
          <el-button type="primary" style="width:100%" plain>点击登陆</el-button>
        </el-form-item>
      </el-form>
    </el-card>
  </div>
</template>

<script>
export default {
  data () {
    return {
      from: {
        name: ''
      }
    }
  }
}
</script>

<style scoped lang='less'>
.bgc {
  width: 100%;
  height: 100%;
  background: url("../../assets/timg (1).jpg") no-repeat;
  position: absolute;
  left: 0;
  top: 0;
  .el-form-item__content {
    margin-left: 0;
  }
}
.box-card {
  width: 480px;
  height: 350px;
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  img {
    display: block;
    margin: 0 auto 18px;
  }
}
</style>
