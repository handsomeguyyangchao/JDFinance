<template lang="html">
        <div>
            <Welfare/>
            <List/>
            <Base name="实名认证" imgsrc="https://img12.360buyimg.com/jrpmobile/jfs/t10423/230/287832134/1427/af7e4c86/59cb61b2N53280a30.png?width=70&height=70"/>
            <Base name="帮助中心" imgsrc="https://img12.360buyimg.com/jrpmobile/jfs/t9832/294/292213011/2420/30888b3d/59cb61c9Nc2bbc057.png?width=70&height=70" :class="$style.margin"/>
            <!-- <Identification/> -->
            <!-- <Help/> -->
            <Navbar/>
        </div>
    </template>
    
    <script>
    import Welfare from "./welfare.vue"
    import List from "./list.vue"
    import Base from "./base.vue"
    import Navbar from "../public/navbar.vue"
    // import Identification from "./identification.vue"
    // import Help from "./help.vue"
    
    export default {
        components: {
            Welfare,
            List,
            Base,
            // Identification,
            // Help
            Navbar

        },
    }
    </script>
    <style lang="scss" module>
    .margin{
        margin-bottom:120px !important;
    }
    </style>
    
    
