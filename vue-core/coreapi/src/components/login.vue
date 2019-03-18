<template>
  <div class="login">
        <el-row :gutter="20">
            <el-col :span="12" :offset="6">
                <el-tabs type="border-card">
                    <el-tab-pane label="登录">
                        <loginComponent></loginComponent>
                    </el-tab-pane>
                    <el-tab-pane label="注册">
                        <registerComponent></registerComponent>
                    </el-tab-pane>
                </el-tabs>
            </el-col>
        </el-row>
        
  </div>
</template>

<script>
import loginComponent from '@/components/loginComponent'
import registerComponent from '@/components/registerComponent'
export default {
  name: 'login',
  components: {
      loginComponent,
      registerComponent
  },
  data() { 
    return {

    }
  },

 }
</script>
<style scoped>

</style>
