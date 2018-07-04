<template>
<div class="wrapper">
  <swiper :options="swiperOption" >
    <swiper-slide v-for="item of swiperList" :key='item.id'>
        <img class="swiper-img" :src="item.imgUrl" />
    </swiper-slide>
    <div class="swiper-pagination"  slot="pagination"></div>
  </swiper>
</div>
</template>

<script>
export default {
    name:'HomeSwiper',
    data () {
        return {
            swiperOption: {
                pagination:'.swiper-pagination',
                loop:true
            },
            swiperList:[{
                id:'001',
                imgUrl:'http://img1.qunarzz.com/piao/fusion/1806/8f/d09fa241a01ac02.jpg_750x200_e0c86013.jpg'
            },{
                id:'002',
                imgUrl:'http://img1.qunarzz.com/piao/fusion/1805/3b/ef86879aa50e3002.jpg_750x200_2a108508.jpg'
            },{
                id:'003',
                imgUrl:'http://img1.qunarzz.com/piao/fusion/1806/60/2eee57f623edfa02.jpg_750x200_74566baa.jpg'
            }]
        }
    }
}
</script>

<style lang='stylus' scoped>
.wrapper >>> .swiper-pagination-bullet-active
 background:#fff
.wrapper
 overflow :hidden
 width:100%
 height:0
 padding-bottom:26.67%
 background:#eee
 .swiper-img
  width:100%
</style>
