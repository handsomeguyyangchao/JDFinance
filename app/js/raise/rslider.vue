<template lang="html">
    <Panel :class="$style.panel">
        <section :class="$style.content">
            <Slider :items="items"></Slider>
        </section>  
        
    </Panel>
</template>

<script>
import Slider from '../core/slider.vue'
import Panel from '../core/panel.vue'
export default {
  data() {
    return {
        items:[{
            href:"raise",
            src:"https://img12.360buyimg.com/jrpmobile/jfs/t1/10771/15/10112/59421/5c52d9b0Ef5d246dc/11ad1847556378f3.jpg?width=750&height=360"
        },
        {
            href:"raise",
            src:"https://img12.360buyimg.com/jrpmobile/jfs/t1/28679/13/11666/46495/5c919c52Ec49527f1/137c903aa051210d.jpg?width=750&height=360"
        },{
            href:"raise",
            src:"https://img12.360buyimg.com/jrpmobile/jfs/t1/18086/11/11008/106906/5c8b4affEe67adbca/e29a811f999f4d58.jpg?width=750&height=360"
        }
        ,{
            href:"raise",
            src:"https://img12.360buyimg.com/jrpmobile/jfs/t1/25366/33/11885/26672/5c9392a8Ecf8c20ea/6077d96740663912.jpg?width=750&height=360"
        }]
    }
  },
  components: {
      Panel,
      Slider
  }
}
</script>


<style lang="scss" module>
@import '../../css/element.scss';
.panel{
    @include panel;
    margin-top:3rem;
    >h4{
        display: none;
    }
    .content{
        margin-top: 120px;
    }
}

</style>
