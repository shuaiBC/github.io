<template>
  <div class="index">
    <div :style="{background: '#102131'}">
      <div class="indexHeader">
        <!-- <a-affix :offsetTop="10" @change="change"></a-affix> -->
        <a-row class="header">
          <a-col :span="8">
            <a class="underline">首页</a>
            <a :style="{marginLeft: '50px'}" class="underline">技术博客</a>
          </a-col>
          <a-col :style="{textAlign: 'center'}" :span="8">
            <h3 :style="{color: '#fff'}">Zoo Team大前端基础设施平台</h3>
          </a-col>
          <a-col :style="{textAlign: 'right'}" :span="8">
            <a-button type="primary">点击按钮</a-button>
          </a-col>
        </a-row>
        <a-row>
          <a-col :span="12">
            <h1 :style="{fontSize: '47px', marginBottom: '30px', color: '#fff'}">Zoo Team大前端技术平台</h1>
            <p :style="{fontSize: '16px', lineHeight: '30px', maxWidth: '560px'}">tinper 致力于为企业客户和个人开发者提供快速构建泛端应用的服务和能力，其中包含了完整的开发框架、公共SDK以及配套的开发服务，用友网络大前端团队为您提供技术服务。</p>
          </a-col>
          <a-col :span="12">
            <img src="http://tinper.org/assets/images/development.png" alt="">
          </a-col>
        </a-row>
      </div>
    </div>
    <div class="listBackground">
      <List :list="this.list" />
    </div>
    <List :list="this.list1" />
    <NewList />
    <NewState />
    <Footer />
  </div>
</template>

<script>
import NewState from '~/components/newState.vue'
import List from '~/components/list.vue'
import NewList from '~/components/newList.vue'
import Footer from '~/components/footer.vue'

export default {
  name: 'index',
  data() {
    return {
      list: [{
          title: '前端安装包',
          content: '一款快速、安全、可统计的包安装管理平台。',
          icon: '',
        }, {
          title: 'MOCK在线数据服务',
          content: '旨在为开发、产品、测试人员提供更优雅的接口管理服务。',
          icon: '',
        }, {
          title: 'CDN公共资源',
          content: '公共资源静态资源库公共资源静态资源库',
          icon: '',
        }, {
          title: 'Code Guide开发规范',
          content: '用友云前端开发规范',
          icon: '',
        }, {
          title: 'Code Guide开发规范',
          content: '用友云前端开发规范',
          icon: '',
        }, {
          title: 'Code Guide开发规范',
          content: '用友云前端开发规范',
          icon: '',
        }, {
          title: 'Code Guide开发规范',
          content: '用友云前端开发规范',
          icon: '',
        }],
      list1: [{
        title: '前端安装包',
        content: '一款快速、安全、可统计的包安装管理平台。',
        icon: '',
      }, {
        title: 'MOCK在线数据服务',
        content: '旨在为开发、产品、测试人员提供更优雅的接口管理服务。',
        icon: '',
      }, {
        title: 'CDN公共资源',
        content: '公共资源静态资源库公共资源静态资源库',
        icon: '',
      }]
    }
  },
  methods: {
    // change(affixed) {
    //   console.log(affixed)
    // }
  },
  components: {
    NewState,
    List,
    NewList,
    Footer
  }
}
</script>

<style lang="scss" scoped>
.index {
  background: #fff;
  .indexHeader {
    width: 84%;
    position: relative;
    margin: auto;
    color: #fff;
  }
  .header{
    height: 100px;
    line-height: 100px;
    .underline{
      color: #fff;
      position: relative;
      transition-timing-function: ease;
      transition-duration: .3s;
      transition-property: left,right,color;
      cursor: pointer;
    }
    .underline:after{
      content: "";
      position: absolute;
      left: 50%;
      right: 50%;
      top: 25px;
      background: #1890ff;
      height: 2px;
      transition-property: left,right;
      transition-property: left,right;
      -webkit-transition-property: left,right;
      transition-duration: .3s;
      -webkit-transition-duration: .3s;
      transition-timing-function: ease-out;
      -webkit-transition-timing-function: ease-out;
    }
    .underline:hover{
      font-weight: 300;
      color: #1890ff;
    }
    .underline:hover:after{
      left: 0;
      right: 0;
    }
  }
  .listBackground {
    background: url('http://tinper.org/assets/images/background2.jpg') center -40px no-repeat;
  }
}
</style>
