<template lang="html">
    <Panel title="会员福利" :class="$style.panel">
        <section :class="$style.content">
            <div :class="$style.left">
                <img :src="imgsrc" alt="">
                <span>{{name}}</span>
            </div>
            <div :class="$style.right"></div>
        </section>
    </Panel>
</template>

<script>
import Panel from "../core/panel"
export default {
  data() {
    return {
      
    }
  },
  components: {
      Panel
  },
  props:{
      name:{
          type:String,
          default:''

      },
      imgsrc:{
          type:String,
          default:''
      }
  }
}
</script>

<style lang="scss" module>
@import "../../css/element.scss";
.panel{
  @include panel;
  margin-top:0!important;
  >h4{
    display:none;
  }
  .content{
    @include flex(row);   
    background:url(//m.jr.jd.com/spe/qyy/main/images/icon_arrow1.png) 95% center no-repeat;
    justify-content: space-between;
    height:112px;
    line-height: 112px;
    .left{
      @include flex(row);
      justify-content:flex-start;
      align-items: center;
      height:112px;
      line-height: 112px;
      margin-left: 32px;
      box-sizing: border-box;
      img{
          display: inline-block;
          width:48px;
          height:48px;
          line-height: 112px;
        }
        span{
            margin-left: 30px;
            font-size: 32px;
            color: #333;
            display: block;
            white-space: nowrap;
            text-overflow: ellipsis;
            overflow: hidden;
        }
    }
    .right{
      height:140px;
      line-height: 140px;
      font-size:28px;
      color:#999;
      box-sizing: border-box;
      margin-right: 65px;
    }

  }

}
</style>
