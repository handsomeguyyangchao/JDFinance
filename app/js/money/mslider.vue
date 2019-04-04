<template lang="html">
    <Panel title="理财精选" :class="$style.panel">
        <section :class="$style.content">
            <Slider :items="items" :cname="$style.slider"></Slider>
        </section>
        
    </Panel>
</template>

<script>
import Panel from "../core/panel";
import Slider from "../core/slider";
export default {
  data() {
    return {
        items:[{
            src:"//img12.360buyimg.com/jrpmobile/jfs/t1/16015/18/9611/64227/5c9830a4E756251d6/67f2ffa3ea918d59.png?width=750&height=400",
            name:"a1",
        },{
            src:"//img12.360buyimg.com/jrpmobile/jfs/t1/11337/12/12145/120426/5c8f2926Ea9d776bf/8f2fc4a4c1d465ce.jpg?width=750&height=400",
            name:"a2"
        },{
            src:"//img12.360buyimg.com/jrpmobile/jfs/t1/19924/31/11803/148725/5c9331cbE51a3d388/130a88da462400a7.png?width=750&height=400",
            name:"a3"
        }],
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
    >h4{
        display:none;
    }
    .content{
        margin-top: 3rem;
    }
    ul{
        @include flex(row);
        li{
            width: 20%;
            box-sizing:border-box;
            img{
                box-sizing:border-box;
                width:90px;
                height: 90px;
                text-align: center;
            }
            p{
                color:#ddd;
                font-size:24px;
                text-align: center;
            }
        }
        
    }
    
}
</style>