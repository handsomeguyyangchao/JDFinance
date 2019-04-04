<template lang="html">
    <Panel title="借钱新人" :class="$style.panel">
        <section :class="$style.content">
            <img src="//img12.360buyimg.com/jrpmobile/jfs/t1/32160/39/7247/126113/5c94d7d7E1621a616/a35e308781c8741d.jpg?width=750&height=200" alt="">
        </section>
    </Panel>
</template>

<script>
import Panel from '../core/panel';
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
@import '../../css/element.scss';
.panel{
  @include panel;
  >h4{
    display:none;
  }
  .content{
      img{
        width: 100%;
        height: 4.25rem;
        display: block;
      }
    }
}

</style>
