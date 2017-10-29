<template>
  <div class="episode swiper-container" id="swiperEpisode">
    <swiper :options="swiperOptionh" >
      <swiper-slide class="slide-h">Horizontal Slide 1
        <swiper :options="swiperOptionv">
          <swiper-slide class="slide-v">Vertical Slide 1</swiper-slide>
          <swiper-slide class="slide-v">Vertical Slide 2</swiper-slide>
          <swiper-slide class="slide-v">Vertical Slide 3</swiper-slide>
          <swiper-slide class="slide-v">Vertical Slide 4</swiper-slide>
          <swiper-slide class="slide-v">Vertical Slide 5</swiper-slide>
          <div class="swiper-pagination swiper-pagination-v" slot="pagination"></div>
        </swiper>
      </swiper-slide>
      <swiper-slide class="slide-h">Horizontal Slide 2
        <swiper :options="swiperOptionv">
          <swiper-slide class="slide-v">Vertical Slide 1</swiper-slide>
          <swiper-slide class="slide-v">Vertical Slide 2</swiper-slide>
          <swiper-slide class="slide-v">Vertical Slide 3</swiper-slide>
          <swiper-slide class="slide-v">Vertical Slide 4</swiper-slide>
          <swiper-slide class="slide-v">Vertical Slide 5</swiper-slide>
          <div class="swiper-pagination swiper-pagination-v" slot="pagination"></div>
        </swiper>
      </swiper-slide>
      <swiper-slide class="slide-h">Horizontal Slide 3
        <swiper :options="swiperOptionv">
          <swiper-slide class="slide-v">Vertical Slide 1</swiper-slide>
          <swiper-slide class="slide-v">Vertical Slide 2</swiper-slide>
          <swiper-slide class="slide-v">Vertical Slide 3</swiper-slide>
          <swiper-slide class="slide-v">Vertical Slide 4</swiper-slide>
          <swiper-slide class="slide-v">Vertical Slide 5</swiper-slide>
          <div class="swiper-pagination swiper-pagination-v" slot="pagination"></div>
        </swiper>
      </swiper-slide>
      <swiper-slide class="slide-h">Horizontal Slide 4
        <swiper :options="swiperOptionv">
          <swiper-slide class="slide-v">Vertical Slide 1</swiper-slide>
          <swiper-slide class="slide-v">Vertical Slide 2</swiper-slide>
          <swiper-slide class="slide-v">Vertical Slide 3</swiper-slide>
          <swiper-slide class="slide-v">Vertical Slide 4</swiper-slide>
          <swiper-slide class="slide-v">Vertical Slide 5</swiper-slide>
          <div class="swiper-pagination swiper-pagination-v" slot="pagination"></div>
        </swiper>
      </swiper-slide>
      <div class="swiper-pagination swiper-pagination-h" slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
  export default {
    name: 'Episode',
    data () {
      return {
        swiperOptionh: {
          pagination: '.swiper-pagination-h',
          paginationClickable: true,
          direction: 'horizontal'
        },
        swiperOptionv: {
          pagination: '.swiper-pagination-v',
          paginationClickable: true,
          direction: 'vertical',
          spaceBetween: 10
        }
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" rel="stylesheet/scss">
  .episode{
    width:100%;
    /*height:300px;*/
    background: #ccc;
  }
  .slide-h{
    /*border:1px solid red;*/
  }
  .slide-v{
    border:1px solid green;
    background: url("http://via.placeholder.com/300x300");
    background-size: cover;
    /*width:100%;*/
    /*height:300px;*/
  }
  .swiper-container-v {
    background: #eee;
  }
</style>
