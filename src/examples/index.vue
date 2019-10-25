<template>
  <div class="home-container">
    <div class="Header">图片预览组件</div>
    <div class="item-wrapper">
       <div class="item-image">
         <ap-image :showClose="false" :thumb="imgUrl" :radius="3" :full="imgUrl" :maxWidth="300"></ap-image>
       </div>
       <div class="item-right">
          <div style="font-size:3.6vw;">新闻标题图片预览组件</div>
          <div style="font-size:3.4vw;color:#777;">描述</div>
       </div>
    </div>

  </div>
</template>

<script>

export default {
  name: 'el-index',
  components: {
  },
  data () {
    return {
      imgUrl: 'http://data618.oss-cn-qingdao.aliyuncs.com/ys/3524/img/b.jpg'
    };
  },
  mounted () {
    console.log('mounted');
  }
};
</script>

<style lang="scss" scoped>
.tab {
  text-align: center;
  padding: 10px;
  margin: 5px 0;
  background-color: #F2F2F2;
  a {
    color: #7e8c8d;
  }
}

  .home-container{
    width: 100%;

    .Header{
      background:linear-gradient(90deg, rgb(231, 86, 142), #ff696b);
      padding: 4vw;
      color: #fff;
      text-align: center;
    }
    .item-wrapper{
      display: flex;
      padding: 4vw;
    }
    .item-image{  
      width: 25vw;
    }
    .item-right{
      flex: 1;
      margin-left: 3vw;
      display: flex;
      justify-content: space-between;
      flex-direction: column;
      padding: 1vw 0;
    }
  }
</style>
