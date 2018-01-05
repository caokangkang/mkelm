<template>
 <div class="page">
     <span class="icon"></span>
 </div>
</template>

<script type="text/ecmascript-6">
 export default {
   data () {
     return {

     };
   },
   components: {

   }
 };
</script>

<style scoped lang="stylus">
  .icon
    display: inline-block
    vertical-align: top
    width: 12px
    height: 12px
    margin-right: 2px
    background-size: 12px 12px
    background-repeat: no-repeat
    &.decrease
      bg-image('decrease_3')
    &.discount
      bg-image('discount_3')
    &.guarantee
      bg-image('guarantee_3')
    &.invoice
      bg-image('invoice_3')
    &.special
      bg-image('special_3')
</style>
