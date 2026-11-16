<template>
  <div class="header">
    <el-row :gutter="20" style="width: 1400px; margin: 0 auto">
      <el-col :span="6">
        <div class="logo-box">
          <img
            alt="安徽壹鑫"
            class="yixin-logo"
            src="@/assets/img/logo.png"
            height="50"
          />
          <span class="name">安徽壹鑫</span>
        </div>
      </el-col>
      <el-col :span="18" style="margin-top: 10px">
        <el-menu
          :default-active="activeIndex"
          class="el-menu-demo"
          mode="horizontal"
          @select="handleSelect"
          active-text-color="#409eff"
          :router="true"
        >
          <el-menu-item index="index">首页</el-menu-item>
          <!-- <el-menu-item index="index2">公司介绍</el-menu-item> -->
        </el-menu>
      </el-col>
    </el-row>
  </div>
</template>
<script setup>
const props = defineProps({
  activeIndex: {
    type: String,
    default: "index",
  },
});
</script>
<style scoped lang="less">
.header {
  height: 84px;
  position: fixed;
  width: 100%;
  top: 0;
  left: 0;
  z-index: 999;
  background: #fff;
  display: flex;
  align-items: center;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}
.logo-box {
  display: flex;
  align-items: center;
  margin-top: 10px;

  .yixin-logo {
    margin: 0 10px;
  }

  .name {
    font-size: 28px;
    font-weight: 600;
    color: @primary-color;
  }
}

.el-menu-item {
  padding: 0 10px !important;
  margin: 0 20px !important;
  font-size: 16px !important;
}
.el-submenu__title {
  padding: 0 10px !important;
  margin: 0 30px !important;
  font-size: 16px !important;
}
.el-menu--horizontal > .el-submenu .el-submenu__title {
  height: 50px !important;
  line-height: 50px !important;
}
.el-menu--horizontal > .el-menu-item.is-active {
  font-weight: bold !important;
  border-bottom: 4px solid #409eff !important;
}
.el-menu--horizontal > .el-submenu.is-active .el-submenu__title {
  font-weight: bold !important;
  border-bottom: 4px solid #409eff !important;
}
.el-menu.el-menu--horizontal {
  border: none !important;
}
.el-menu--horizontal > .el-menu-item {
  height: 50px !important;
  line-height: 50px !important;
}
.el-menu--horizontal > .el-submenu.is-active .el-submenu__title i {
  color: #409eff !important;
}

.el-menu-item:hover {
  background-color: #ffffff !important;
}
</style>
