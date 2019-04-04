<template lang="html">
    <Panel title="今日推荐" :cname="$style.panel">
        <section>
          <Slider :options="options" :items="items" cname="today-product-slider" ></Slider>
        </section>
    </Panel>
</template>

<script>
import Panel from '../core/panel.vue';
import Slider from '../core/slider.vue'
export default {
  data() {
    return {
        items: [{
                href: "money",
                src: "//img12.360buyimg.com/jrpmobile/jfs/t17536/263/1512937672/326395/36043d78/5acd6d54N3c6bde4d.jpg",
            }, {
                href: "money",
                src: "//img12.360buyimg.com/jrpmobile/jfs/t22615/244/823832818/267495/95c6b15/5b42c775N13a85fd7.jpg",
            }, {
                href: "money",
                src: "//img12.360buyimg.com/jrpmobile/jfs/t1/7840/16/5560/153378/5bde93b1E0c835ca0/6b634ff3b6954ebe.jpg",
            }, {
                href: "money",
                src: "//img12.360buyimg.com/jrpmobile/jfs/t29302/317/288992565/369473/eff76296/5bee40c6N09b4b0d0.jpg",
            }, {
                href: "money",
                src: "//img12.360buyimg.com/jrpmobile/jfs/t1/20010/2/6861/79405/5c6389bfE5eaa92b9/56afaa4c884f0e22.jpg",
            }, {
                href: "money",
                src: "//img12.360buyimg.com/jrpmobile/jfs/t16171/262/1244648454/676912/5d19a4cb/5a52da5cN18d30d9f.jpg",
            }],
        options: {
            slidesPerView: 2.3,
            spaceBetween: 30,
            freeMode: true,
        },
    }
  },
  components: {
      Panel,
      Slider
  }
}
</script>
<style lang="scss">
  .today-product-slider{
    .swiper-container{
      box-sizing: border-box;
      padding: 0 24px;
      .swiper-slide{
        a{
          display: inline-block;
          width: 100%;
          img{
            width: 100%;
            display: block;
            height: 314px;
            border: 1px solid #fafafa;
          }
        }
      }
    }
  }
</style>

<style lang="scss" module>
@import '../../css/element.scss';
.panel{
    @include panel;
    .content{
      padding-bottom: 40px;
      position: relative;
      
    }
  }

</style>


