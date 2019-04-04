<template lang="html">
    <Panel title="会员福利" :class="$style.panel">
        <section :class="$style.content">
            <div :class="$style.left">
              
            </div>
            <div :class="$style.right">
              会员福利
            </div>
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
    justify-content: space-between;
    align-items: center;
    background:url(//m.jr.jd.com/spe/qyy/main/images/icon_arrow1.png) 95% center no-repeat;
    height:140px;
    .left{
      width:100px;
      height:140px;
      margin-left: 32px;
      box-sizing: border-box;
      background:url(https://img12.360buyimg.com/jrpmobile/jfs/t2644/238/1420176553/1442/96e2885/573d96deN06201af5.png) center center no-repeat;
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
