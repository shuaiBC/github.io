<template>
  <div class="newState">
    <a-row class="content">
      <a-col class="newState_col" :span="8">
        <img class="newState_img" src="http://tinper.org/assets/images/weChat.png" alt="">
        <div class="newState_left">
          <p class="newState_left_content">问题反馈</p>
          <p>扫描二维码，加入官方技术交流群</p>
        </div>
      </a-col>
      <a-col class="newState_col newState_col_left" :span="8">
        <a-icon :style="{fontSize: '46px'}" type="github" />
        <div class="newState_left">
          <p class="newState_left_content">Github 地址</p>
          <p>https://github.com/iuap-design</p>
        </div>
      </a-col>
      <a-col class="newState_col newState_col_left" :span="8">
        <a-icon :style="{fontSize: '46px'}" type="disconnect" />
        <div class="newState_left">
          <p class="newState_left_content">相关链接</p>
          <p>http://design.yyuap.com/</p>
        </div>
      </a-col>
    </a-row>
  </div>
</template>

<script>
export default {
  name: 'newState',
}
</script>

<style lang='scss' scoped>
.newState {
  background-color: #F8FAFD;
  padding: 20px 20px 10px 20px;
  .content {
    width: 84%;
    position: relative;
    margin: auto;
    .newState_col {
      height: 140px;
      text-align: center;
      .newState_img {
        width: 120px; 
        height: 130px;
        vertical-align: center;
      }
      .newState_left {
        display: inline-block;
        margin-left: 10px;
        .newState_left_content {
          text-align: left;
        }
      }
    }
    .newState_col_left {
      padding-top: 16px;
    }
  }
}
</style>
