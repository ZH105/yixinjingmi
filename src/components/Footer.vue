<template>
  <div class="footer">
    <div class="logo-box">
      <img
        alt="安徽壹鑫"
        class="yixin-logo"
        src="@/assets/img/logo.png"
        height="50"
      />
      <span class="name">安徽壹鑫</span>
    </div>
    <div class="info-box">
      <div class="info-item">
        <div class="info-tab">公司地址</div>
        <div>安徽省池州市青阳县木瓜山路木镇工业园区</div>
      </div>
      <div class="info-item">
        <div class="info-tab">联系方式</div>
        <div>电话：123456789</div>
        <div>邮箱：123456789@qq.com</div>
      </div>
    </div>
  </div>
</template>
<style scoped lang="less">
.footer {
  height: 130px;
  background-color: @primary-color;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 20px 50px;

  .logo-box {
    display: flex;
    align-items: center;
    .yixin-logo {
      margin-right: 10px;
    }
    .name {
      color: #fff;
      font-size: 24px;
    }
  }

  .info-box {
    display: flex;
    align-items: flex-start;
    gap: 50px;

    .info-item {
      color: #fff;
      font-size: 14px;

      .info-tab {
        font-size: 16px;
        font-weight: 600;
        margin-bottom: 10px;
      }
    }
  }
}
</style>
