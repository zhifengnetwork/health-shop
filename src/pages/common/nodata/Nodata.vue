<template>
    <div class="nodata-wrap">
        <img class="-info-img" :src="nodatas.imgSrc"/>
        <p class="-info-txt">{{nodatas.text}}~</p>
        <router-link :to="nodatas.link"><input class="-info-btn" type="button" value="去逛逛" /> </router-link>
    </div>
</template>
<script>
    export default {
        props:{
            nodatas:{
                type:Object,
                required:true
            }
        }
    }
</script>

<style lang="stylus" scoped>
    .nodata-wrap
        text-align :center
        .-info-img
            width:290px
            height:290px
            margin:145px 0 50px
        .-info-txt
            color:#6c6c6c
            font-size:36px
            margin-bottom:90px
        .-info-btn
            width: 460px
            height: 100px
            background: #ea2028
            border-radius: 50px
            font-size 50px
            color:#fff
</style>

