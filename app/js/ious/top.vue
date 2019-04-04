<template lang="html">
    <Panel title="借贷登录" :class="$style.panel">
        <section :class="$style.content">
            <div :class="$style.card">

            </div>
            <p :class="$style.login">立即登录</p>
            <Slider :options="options" :items="items" cname="top-slider"></Slider>
        </section>
    </Panel>
</template>

<script>
import Panel from "../core/panel.vue";
import Slider from "../core/slider.vue";
export default {
  data() {
    return {
        options:{
                    autoplay: true,
                    loop: true,
                    pagination: {
                        el: ".swiper-pagination",
                    },
                    notNextTick: false,
                },
        items:[{
            src:"//img12.360buyimg.com/jrpmobile/jfs/t1/6758/25/12426/30531/5c3327b7Ea2d96add/3cbcac830338b901.png?width=1080&height=240",
            href:"ious"
        },{
            src:"//img12.360buyimg.com/jrpmobile/jfs/t1/26962/32/8709/86856/5c793513E7b0e9f90/fe79bbc067e90a38.png?width=1080&height=240",
            href:"ious"
        },{
            src:"//img12.360buyimg.com/jrpmobile/jfs/t1/6758/25/12426/30531/5c3327b7Ea2d96add/3cbcac830338b901.png?width=1080&height=240",
            href:"ious"
        }]
    }
  },
  components: {
      Panel,
      Slider
  }
}
</script>

<style>
.top-slider{

}
</style>

<style lang="scss" module>
@import "../../css/element.scss";
.panel{
    @include panel;
    margin-top: 200px;
    // background: url("../../css/img/bj.png") no-repeat 0% 0%;
    >h4{
        display: none;
    }
    .content{
        .card{
            height: 340px;
            border:1px solid #ddd;
            // background: url("../../css/img/goldCard.png") no-repeat 0% 0%;
            position: relative;
        }
        .login{
            position: absolute;
        }

    }
}

</style>
