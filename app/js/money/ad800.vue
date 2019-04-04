<template lang="html">
    <Panel title="最高领800京豆" :class="$style.panel">
        <section :class="$style.content">
            <img src="//img12.360buyimg.com/jrpmobile/jfs/t1/24958/23/5984/66824/5c466c74Eefe11794/234f78a6487d9130.jpg?width=750&height=200" alt="">
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
    >h4{
        display: none;
    }
    .content{
        img{
            display: flex;
            width:100%;
        }
    }
}

</style>
