<template lang="html">
    <Panel title="帮助中心" :class="$style.panel">
        <section :class="$style.content">
            <div :class="$style.welfare"></div>
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

</style>
