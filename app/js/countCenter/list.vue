<template lang="html">
    <Panel title="入口列表"  :class="$style.panel">
        <section :class="$style.content">
            <ul :class="$style.list">
              <li :class="$style.liclass" v-for="(item,key) in items">
                <router-link :to="{name:item.href}">
                  <div :class="$style.left">
                    <img :src="item.src" alt="">
                    <span>{{item.name}}</span> 
                  </div>
                  <div :class="$style.right">
                    {{item.title}}
                  </div>
                </router-link>
              </li>
            </ul>
        </section>
    </Panel>
</template>

<script>
import Panel from "../core/panel";

export default {
  data() {
    return {
      items:[
        {
          "src":"https://img12.360buyimg.com/jrpmobile/jfs/t8971/199/1863233880/2035/56d04776/59cb5fbdNa7c682c3.png?width=70&height=70",
          "name":"我的资产",
          "title":"查看全部资产",
          "href":"download",
        },{
          "src":"https://img12.360buyimg.com/jrpmobile/jfs/t8836/18/2342020923/2120/a9b7a8ff/59cb6124N31cb2889.png?width=70&height=70",
          "name":"我的优惠券",
          "title":"查看全部",
          "href":"download"
        },{
          "src":"https://img12.360buyimg.com/jrpmobile/jfs/t10264/48/2521964269/2177/cb479501/59f945edNc1197b64.png?width=90&height=90",
          "name":"我的金币",
          "title":"赚金币兑好物",
          "href":"download"
        },{
          "src":"https://img12.360buyimg.com/jrpmobile/jfs/t12115/250/469950434/3906/ad97c994/5a0bdf3aN22efb724.png?width=90&height=90",
          "name":"我的金条",
          "title":"查看额度",
          "href":"download"
        },{
          "src":"https://img12.360buyimg.com/jrpmobile/jfs/t9244/132/2364556535/1134/334cd5d9/59cb612dN5b974dc5.png?width=70&height=70",
          "name":"我的借钱",
          "title":"查看全部产品",
          "href":"download"
        },{
          "src":"https://img12.360buyimg.com/jrpmobile/jfs/t9121/110/2300703915/1348/91af205c/59cb613bN1e749e58.png?width=70&height=70",
          "name":"我的白条",
          "title":"去提额",
          "href":"download"
        },{
          "src":"https://img12.360buyimg.com/jrpmobile/jfs/t9649/171/293125950/1453/4cf0cc2/59cb6162N9c71da0f.png?width=70&height=70",
          "name":"我的众筹",
          "title":"查订单/物流",
          "href":"download"
        },{
          "src":"https://img12.360buyimg.com/jrpmobile/jfs/t8014/149/2344686222/2102/341ff316/59cb616bN3e1bd87d.png?width=70&height=70",
          "name":"我的保障",
          "title":"全方位保障",
          "href":"download"
        },{
          "src":"https://img12.360buyimg.com/jrpmobile/jfs/t1/3907/34/11652/2582/5bd04759Ea9acb837/f893bf98fd67c192.png?width=54&height=54",
          "name":"我的爱车",
          "title":"绑车享专属福利",
          "href":"download"
        },
      ]
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
    ul.list{
      .liclass{
          a{
          text-decoration: none;
          @include flex(row);
          justify-content: space-between;
          align-items: center;
          background:url(//m.jr.jd.com/spe/qyy/main/images/icon_arrow1.png) 95% center no-repeat;
          height:112px;
          line-height: 112px;
          position: relative;
          &:after{
            content:" ";
            display:block;
            width:534px;
            height:0;
            border-top:1px solid #eee;
            position: absolute;
            bottom:0;
            right:0;
          }
          .left{
            box-sizing: border-box;
            font-size: 32px;
            color: #333;
            white-space: nowrap;
            text-overflow: ellipsis;
            overflow: hidden;
            margin-left: 32px;
            display: flex;
            align-items: center;
            img{
              display: inline-block;
              width:48px;
              height:48px;
              line-height: 112px;
            }
            span{
              margin-left: 30px;
            }
          }
          .right{
            font-size:28px;
            color:#999;
            box-sizing: border-box;
            margin-right: 65px;
            white-space: nowrap;
            text-overflow: ellipsis;
            overflow: hidden;
          }
          
        }
        &:last-child{
            .right{
              color: #FF801A;
            }
          }
      }
    }
    
  }

}

</style>
