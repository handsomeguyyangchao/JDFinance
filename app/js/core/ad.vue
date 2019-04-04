<template lang="html">
    <Panel title="广告基础组件" :class="$style.panel">
        <section>
            <img :src="imgSrc" alt="" :class="[baseClass,adClass]">
        </section>
    </Panel>
</template>

<script>
import Panel from './panel.vue';
export default {
  data() {
    return {
        baseClass:{
            padding:'9px',
        }
    }
  },
  components: {
      Panel
  },
  props:{
      imgSrc:{
          default(){
              return "路径错误"
          }
      },
    //   adClass:{
    //       default(){
    //           return {
    //               "padding":'10'
    //               }
    //       }
    //   }
    adClass:{
        type:String,
        default:""
    }
  }
}
</script>

<style lang="scss" module>
@import '../../css/element.scss';
.panel{
    @include panel;
    >h4{
        display: none;
    }
    img{
        display: flex;
        width: 100%
    }
}

</style>
