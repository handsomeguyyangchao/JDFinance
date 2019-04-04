<template lang="html">
        <div>
            <Heador/>
            <Slider/>
            <Novice/>
            <Borrow/>
            <Product/>
            <Life/>
            <Footor/>
            <Navbar/>
            <!-- <Money/>
            -->
        </div>
    </template>
    
    <script>
    import Heador from "../public/header.vue"
    import Footor from "../public/footer.vue"
    import Navbar from "../public/navbar.vue"
    import Slider from "./hslider.vue"
    import Novice from "./novice.vue"
    import Borrow from "./borrow.vue"
    // import Money from "./money.vue"
    import Product from "./product.vue"
    import Life from "./life.vue"
    export default {
        components: {
            Heador,
            Slider,
            Novice,
            Borrow,
            Product,
            // Money,
            Life,
            Footor,
            Navbar,
        },
    }
    </script>
    
