<template>
  <div class="newList">
    <h5>这里是标题</h5>
    <a-row class="newListRow">
      <a-col v-for="(item, index) in list" :key="index" :span="8">
        <a class="newListRowTitle">
          <a-icon type="safety" />
          <a-tooltip placement="topLeft" >
            <template slot="title">
              <span :title="item.content">【{{item.title}}】{{item.content}}</span>
            </template>
            <span :title="item.content">【{{item.title}}】{{item.content}}</span>
          </a-tooltip>
        </a>
      </a-col>
    </a-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      list:[{
        title: 'tinper-sparrow',
        content: '修改项目目录命名规范，统一为小写，遇到需要连接的统一用“-”，组件文件名统一遵循大驼峰命名。',
      }, {
        title: 'tinper-sparrow',
        content: '修改项目目录命名规范，统一为小写，遇到需要连接的统一用“-”，组件文件名统一遵循大驼峰命名。',
      }, {
        title: 'tinper-sparrow',
        content: '修改项目目录命名规范，统一为小写，遇到需要连接的统一用“-”，组件文件名统一遵循大驼峰命名。',
      }, {
        title: 'tinper-sparrow',
        content: '修改项目目录命名规范，统一为小写，遇到需要连接的统一用“-”，组件文件名统一遵循大驼峰命名。',
      }, {
        title: 'tinper-sparrow',
        content: '修改项目目录命名规范，统一为小写，遇到需要连接的统一用“-”，组件文件名统一遵循大驼峰命名。',
      }, {
        title: 'tinper-sparrow',
        content: '修改项目目录命名规范，统一为小写，遇到需要连接的统一用“-”，组件文件名统一遵循大驼峰命名。',
      }, {
        title: 'tinper-sparrow',
        content: '修改项目目录命名规范，统一为小写，遇到需要连接的统一用“-”，组件文件名统一遵循大驼峰命名。',
      }, {
        title: 'tinper-sparrow',
        content: '修改项目目录命名规范，统一为小写，遇到需要连接的统一用“-”，组件文件名统一遵循大驼峰命名。',
      }, {
        title: 'tinper-sparrow',
        content: '修改项目目录命名规范，统一为小写，遇到需要连接的统一用“-”，组件文件名统一遵循大驼峰命名。',
      }, {
        title: 'tinper-sparrow',
        content: '修改项目目录命名规范，统一为小写，遇到需要连接的统一用“-”，组件文件名统一遵循大驼峰命名。',
      }, {
        title: 'tinper-sparrow',
        content: '修改项目目录命名规范，统一为小写，遇到需要连接的统一用“-”，组件文件名统一遵循大驼峰命名。',
      }]
    }
  }
}
</script>

<style lang="scss" scoped>
  .newList {
    margin-top: 120px;
    margin-bottom: 80px;
    width: 84%;
    margin-left: 8%; 
    h5{
      font-size: 20px;
      color: red;
      margin-bottom: 16px;
    }
    .newListRow {
      padding: 10px 0;
      font-size: 14px;
      line-height: 46px;
      background-color: #F8FAFD;
      box-shadow: 0 3px 20px 0 rgba(16,33,49,0.14);
      .newListRowTitle {
        display: block;
        color: #636363;
        height: 100%;
        width: 340px;
        overflow: hidden;
        white-space: nowrap;
        text-overflow: ellipsis;
        font-size: 16px;
        font-style: normal;
        margin: 0;
        border-bottom: 1px dashed #ededed;
        padding: 0 16px;
      }
      .newListRowTitle:hover {
        color:turquoise;
      }
    }
  }
</style>