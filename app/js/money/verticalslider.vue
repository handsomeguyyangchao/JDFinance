<template lang="html">
    <Panel title="垂直轮播" :class="$style.panel" class="vertpanel">
        <div :class="$style.leftDiv">
            <p>6.00</p>
            <p>历史年化收益率</p>
            <p>立即抢购</p>
        </div>
        
        <Slider :options="options" :items="items"  :cname="$style.verticalSlider" >
            <template v-slot="{itemtext}">
                <p>{{ itemtext.text }}</p>
            </template>
        </Slider>
        <div :class="$style.fixed">
            <span>为您推荐</span>
            <!-- <img alt="" src="app/css/img/weinituijianxiayibu.png"> -->
        </div>
    </Panel>
</template>

<script>
import Panel from "../core/panel.vue";
import Slider from "../core/slider";
export default {
  data() {
    return {
        options:{
            autoplay: true,
            direction: 'vertical',
            loop: true,
            notNextTick: false,
        },
        items:[{
            src:"//img12.360buyimg.com/jrpmobile/jfs/t1/7689/1/14465/10585/5c64d790E0b39e2d6/18cb423a372edca4.jpg?width=160&height=160",
            text:'智能电动打气筒 立省180元'
        },{
            src:"//img12.360buyimg.com/jrpmobile/jfs/t1/20022/17/7059/7533/5c64d801E8d1ffa7f/17cca0e28a813d37.jpg?width=160&height=160",
            text:'石墨烯乳胶助眠枕 直降699元'
        },{
            src:"//img12.360buyimg.com/jrpmobile/jfs/t1/24463/16/6972/9020/5c64d815E0cf15a10/5b786ef4c41366bd.jpg?width=160&height=160",
            text:'智能感应净水龙头 立省200元'
        },]
    }
  },
  components: {
      Panel,
      Slider
  }
}
</script>
<style>
.vertpanel .swiper-wrapper{
    height: 200px;
    width:360px;
    box-sizing:content-box;
}
.vertpanel .swiper-slide{
    background: rgb(91, 121, 247)
}
.vertpanel .swiper-slide a{
    display: flex;
    flex-direction: column;

}
.vertpanel .swiper-slide a img{
    width:200px;
    padding: 20px;
    box-sizing:border-box;
}   
.vertpanel .swiper-slide a p{
    position: absolute;
    left: 200px;
    top: 0.75rem;
    color:#fff !important;
    font-size:24px;
}
</style>

<style lang="scss" module>

@import "../../css/element.scss";
.panel{
    @include panel;
    @include flex(row);
    padding: 20px 0;
    position: relative;
    >h4{
        display: none;
    }
    .left-div{
        box-sizing: border-box;
        width:200px;
        font-family:PingFangSC-Regular;
        color:#fff;
        border-radius:.125rem;
        background-color: #ff6016;
        background-size:cover;
        padding:0 38px 0 24px ;
        overflow:hidden;
        text-shadow: 0 0 black;
        margin-left: 28px;
        p{
            &:nth-child(1){
                font-size:1.5625rem;margin-top:.75rem;margin-bottom:0
            }
            &:nth-child(2){
                font-family: PingFangSC-Regular;
                font-size: .625rem;
                height: .875rem;
                line-height: .875rem;
                padding-bottom: .375rem;
                margin-bottom: .375rem;
                position: relative;
                white-space: nowrap;
                text-overflow: ellipsis;
                overflow: hidden;
            }
            &:nth-child(3){
                width: 100%;
                font-family: PingFangSC-Semibold;
                font-size: .75rem;
                height: 1.0625rem;
                line-height: 1.062rem;
            }
        }
    }
    .verticalSlider{
        margin-left:24px;
    }
    .fixed{
        width: 50%;
        height: 114px;
        position: absolute;
        bottom: 0;
        right: .9375rem;
        pointer-events: none;
        z-index: 1;
        span{
            font-size: 0.6rem;
            color: #fff;
            position: relative;
            left: 4rem;
            top: .8rem;
        }
        img{

        }
    }
    
}

</style>
