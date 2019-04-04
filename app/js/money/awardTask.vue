<template lang="html">
    <Panel title="赏金任务" :cname="$style.panel">
        <section>
          <Slider :options="options" :items="items" cname="award-product-slider" ></Slider>
        </section>
    </Panel>
</template>

<script>
import Panel from '../core/panel.vue';
import Slider from '../core/slider.vue';
export default {
  data() {
    return {
        items: [{
                href: "money",
                src: "//img12.360buyimg.com/jrpmobile/jfs/t26893/316/1416172900/5740/58f20b1e/5bc82e3aN7aa90a89.png?width=210&height=260",
            }, {
                href: "money",
                src: "//img12.360buyimg.com/jrpmobile/jfs/t26767/72/1365822552/8516/2e071d95/5bc82e6eN0be93809.png?width=210&height=260",
            }, {
                href: "money",
                src: "//img12.360buyimg.com/jrpmobile/jfs/t30418/166/1039421072/8983/a6f90d5b/5c04eccbN581f6287.png?width=210&height=260",
            }, {
                href: "money",
                src: "//img12.360buyimg.com/jrpmobile/jfs/t26182/297/1417522782/7864/19181a3b/5bc82ec0N0824153d.png?width=210&height=260",
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
  .award-product-slider{
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


