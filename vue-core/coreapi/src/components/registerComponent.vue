<template>
  <div class="loginComponent">
      <el-form ref="form" :model="form" label-width="80px">
        <el-form-item label="选择角色">
            <el-checkbox-group v-model="form.type">
                <el-checkbox label="个人" name="type"></el-checkbox>
                <el-checkbox label="组织" name="type"></el-checkbox>
            </el-checkbox-group>
        </el-form-item>
        <el-form-item label="用户名">
            <el-input v-model="form.name"></el-input>
        </el-form-item>
        <el-form-item label="验证码">
            <el-input v-model="form.code"></el-input>
        </el-form-item>
        <el-form-item label="密码">
            <el-input v-model="form.pwd"></el-input>
        </el-form-item>
        <el-form-item label="确认密码">
            <el-input v-model="form.confirmpwd"></el-input>
        </el-form-item>
        <el-form-item label="邀请码（选填）">
            <el-input v-model="form.sendCode"></el-input>
        </el-form-item>
        <el-form-item>
            <el-checkbox-group v-model="form.type">
                <el-checkbox label="用户注册协议" name="type"></el-checkbox>
            </el-checkbox-group>
        </el-form-item>
        <el-form-item>
            <el-button type="primary" @click="onSubmit">注册</el-button>
        </el-form-item>
        </el-form>
  </div>
</template>

<script>
export default {
  name: 'loginComponent',
  components: {},
  data() { 
    return {
        form: {
            name: '',
            code:'',
            pwd:'',
            confirmpwd:'',
            sendCode:'',
            type: [],
        }
    }
  },
  methods: {
    onSubmit() {
    console.log('submit!');
    }
  },
  
 }
</script>
<style scoped>
    .loginComponent{float: left;}
</style>
