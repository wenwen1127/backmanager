<template>
<el-tabs v-model="activeName" type="card" @tab-click="handleClick">
  <el-tab-pane label="用户管理" name="first">
    <el-button class="button">
      添加全局关键字
    </el-button>
  </el-tab-pane>
  <el-tab-pane label="配置管理" name="second">配置管理</el-tab-pane>

</el-tabs>
</template>

<script>
export default {
  data() {
    return {
      activeName: 'first'
    };
  },
  methods: {
    handleClick(tab, event) {
      console.log(tab, event);
    }
  }
}
</script>

<style>
.button{
  margin: 5px;
}
</style>
