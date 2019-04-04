<template lang="html">
        <div>
            <Heador/>
            <Slider/>
            <Ada/>
            <Ad388/>
            <RowItem/>
            <Verticalslider/>
            <Today/>
            <Ad800/>
            <AwardTask/>
            <Ad imgSrc="//img12.360buyimg.com/jrpmobile/jfs/t1/7640/35/4322/21318/5bda6023E656cbbbb/b2ddefd7ef80d7aa.png?width=750&height=200" AdClass="[classPenObject]" />
            <Footor/>
            <Navbar/>
        </div>
    </template>
    
    <script>
    import Heador from "../public/header.vue"
    import Footor from "../public/footer.vue"
    import Slider from "./mslider.vue"
    import Ada from "./ada.vue"
    import RowItem from "./rowItem.vue"
    import Ad388 from "./ad388.vue"
    import Verticalslider from "./verticalslider.vue"
    import Today from "./today.vue"
    import Ad800 from "./ad800.vue"
    import AwardTask from "./awardTask.vue"
    import Ad from "../core/ad.vue"

    import Navbar from "../public/navbar.vue"
    export default {
        components: {
            Heador,
            Slider,
            Ada,
            Ad388,
            RowItem,
            Verticalslider,
            Today,
            Ad800,
            AwardTask,
            Ad,
            Footor,
            Navbar,
        },
        data(){
            return {
                //放一些 Ad 组件的自定义样式等
                classPenObject:{
                    "padding":"20px 0 20px 0"
                }
            }

        }
    }
    </script>
    
   <style lang="scss">
    .classPenObject{
        padding:"0"
    }
   
   </style>
   
    
