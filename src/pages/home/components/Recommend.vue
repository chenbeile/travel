<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of reconmendList" :key="item.id">
        <img class="item-img" :src="item.imgUrl" />
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data () {
    return {
      reconmendList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1805/6f/6f885ea8b30c67bca3.water.jpg_200x200_21b03a9c.jpg',
        title: '世界之窗',
        desc: '里面是世界各地的标志性建筑或自然景观微缩版'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1807/99/992c99c98928c509a3.water.jpg_200x200_fc4df6ea.jpg',
        title: '深圳欢乐谷',
        desc: '里面是世界各地的标志性建筑或自然景观微缩版'
      }, {
        id: '0003',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1508/2e/d9363ce50a88c8c5ff5a138c67687cd4.water.jpg_200x200_1c15c8f5.jpg',
        title: '深圳野生动物园',
        desc: '里面是世界各地的标志性建筑或自然景观微缩版'
      }, {
        id: '0004',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1507/64/34362835b4a219af8b36803d31a6380f.water.jpg_200x200_bc5c0452.jpg',
        title: '深圳小梅沙海洋世界',
        desc: '里面是世界各地的标志性建筑或自然景观微缩版'
      }, {
        id: '0005',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1611/97/97dbde6eccdfef72a3.water.jpg_200x200_e0efe6da.jpg',
        title: '东部华侨城',
        desc: '里面是世界各地的标志性建筑或自然景观微缩版'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
@import '~styles/mixins.styl'
.title
 margin-top:.2rem
 line-height: .8rem
 background: #eee
 text-indent: .2rem
.item
 overflow: hidden
 display: flex
 height: 1.9rem
 .item-img
  width: 1.7rem
  height: 1.7rem
  padding: .1rem
 .item-info
  flex: 1
  padding: .1rem
  min-width: 0
  .item-title
   line-height: .54rem
   font-size: .32rem
   ellipsis()
  .item-desc
   line-height: .4rem
   color: #ccc
   ellipsis()
  .item-button
   margin-top: .2rem
   background: #ff9300
   padding: 0 .2rem
   border-radius: .06rem
   color: #fff
</style>
