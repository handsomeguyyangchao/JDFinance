<template lang="html">
    <Panel :class="$style.panel" >
        <section >
            <ul :class="$style.content">
                <li>
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t28189/232/289098066/5076/dfe2d74f/5bee6bb4N4ec4cede.png?width=90&height=90" alt="">
                    <p>领红包</p>
                </li>
                <li>
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t27334/12/1829630702/5159/f8133cd6/5bee6bbdN8606cfbb.png?width=90&height=90" alt="">
                    <p>领福利</p>
                </li>
                <li>
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t27796/46/1836066448/4169/de69ccb0/5bee6bc3N92ca0e60.png?width=90&height=90" alt="">
                    <p>优惠券</p>
                    <!-- <span>30-10</span> -->
                </li>
                <li>
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t27850/30/1789047580/4856/13f8bcb9/5bee6bcbN996fb433.png?width=90&height=90" alt="">
                    <p>领京豆</p>
                </li>
                <li>
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t29131/288/288291507/3943/bed46aef/5bee6bd5Nfc5d5360.png?width=90&height=90" alt="">
                    <p>全部</p>
                </li>
            </ul>
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
@import '../../css/element.scss';
    .panel{
        @include panel;
        >h4{
            display:none;
        }
        .content{
            @include flex(row);
            box-sizing: border-box;
            padding: 40px 0;
            background: #fff;
            li{
                width: 20%;
                text-align: center;
                img{
                    width: 90px;
                    height: 90px;
                }
                p{
                    font-size: 26px;
                    color: #666;
                    text-overflow: ellipsis;
                    white-space: nowrap;
                    overflow: hidden;
                    margin-top: 12px;
                    // &:nth-child(3){
                    //     font-family: PingFangSC-Medium;
                    //     font-size: .5625rem;
                    //     color: #fff;
                    //     width: 2.75rem;
                    //     height: 1.4375rem;
                    //     line-height: 1.0625rem;
                    //     text-align: center;
                    //     position: absolute;
                    //     top: -.3125rem;
                    //     left: 50%;
                    //     background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFcAAAAuCAYAAABd5YVlAAAEvklEQ…JuVhSn5skFoBPURDZQrhB9hO0KaU0wdYXrqeyp1gVsLfofkw2rnUOqZEgAAAAASUVORK5CYII=) 50% no-repeat;
                    //     background-size: 100% 100%;
                    // }
                }
            }
        }
    }

</style>
