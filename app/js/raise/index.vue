<template lang="html">
        <div>
            <Heador/>
            <Slider/>
            <Ad imgSrc="//img12.360buyimg.com/jrpmobile/jfs/t20125/139/377044579/41214/51a08cb6/5b0b947bN916e62ee.jpg?width=1500&height=442" AdClass="[classPenObject]" />
            <Life/>
            <Novice/>
            <Footor/>
            <Navbar/>
        </div>
    </template>
    
    <script>
    import Heador from "../public/header.vue"
    import Footor from "../public/footer.vue"
    import Slider from "./rslider.vue"
    import Ad from "../core/ad.vue"
    import Novice from "./novice.vue"
    import Life from "./life.vue"
    

    import Navbar from "../public/navbar.vue"
    export default {
        components: {
            Heador,
            Slider,
            Ad,
            Novice,
            Life,
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
   
    
