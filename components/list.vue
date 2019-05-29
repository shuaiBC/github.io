<template>
  <div class="list">
    <div class="listHeader">
      <h5>这里是标题</h5>
      <p>提供公共开发服务，包含开发规范、可视化开发服务、在线数据mock服务等</p>
    </div>
    <ul class="list-ul">
      <li class="list-li" v-for="(item, index) in list" :key='index'>
        <a>
          <img class="img" src="http://tinper.org/assets/images/doc.svg" alt="">
          <h6>{{item.title}}</h6>
          <p>{{item.content}}</p>
        </a>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  data() {
    return {
      
    }
  },
  props: {
    list: {
      type: Array,
      require: true,
    },
  },
}
</script>

<style lang="scss" scoped>
  .list{
    width: 84%;
    background: #F8FAFD;
    position: relative;
    margin: auto;
    padding: 40px 0;
    .listHeader {
      padding: 0 40px;
      h5{
        padding: 14px 0 22px 0;
        font-size: 20px;
        color: red;
      }
    }
    .list-ul {
      position: relative;
      right: 0;
      left: 0;
      margin: auto;
      max-width: 1072px;
      border-bottom: 1px solid #ccc;
      padding-bottom: 20px;
      .list-li{
        display: inline-block;
        width: 18%;
        height: 211px;
        background: #fff;
        margin: 20px 20px 0 0;
        border: 1px solid #eee;
        border-radius: 6px;
        overflow: auto;
        a{
          display: block;
          width: 100%;
          height: 100%;
          padding: 23px 30px 16px 30px
        }
        .img {
          width: 39px;
          height: 39px;
        }
        h6 {
          font-size: 16px;
          margin: 17px 0 7px 0;
        }
        p {
          font-size: 12px;
          color: #969699;
        }
      }
    .list-li:hover{
        transition: transform .5s;
        transform: translateY(-5px) scale(1.01);
        box-shadow: 0 1px 18px rgba(0, 0, 0, 0.05), 0 5px 30px rgba(0, 0, 0, 0.01);
      }
    }
  }
</style>