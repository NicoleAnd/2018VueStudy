<template>
  <div class="loginComponent">
      <el-form ref="form" :model="form" label-width="80px">
        <el-form-item label="用户名">
            <el-input v-model="form.name"></el-input>
        </el-form-item>
        <el-form-item label="密码">
            <el-input v-model="form.pwd"></el-input>
        </el-form-item>
        <el-form-item>
            <el-checkbox-group v-model="form.type">
                <el-checkbox label="下次自动登录" name="type"></el-checkbox>
            </el-checkbox-group>
        </el-form-item>
        <el-form-item>
            <el-button type="primary" @click="onSubmit">登录</el-button>
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
          pwd:'',
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
