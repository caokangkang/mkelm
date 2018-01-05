<template>
 <div class="goods">
   <div class="menu-wrapper">
     <ul>
       <li v-for="item in goods" class="menu-item"></li>
     </ul>
   </div>
 </div>
</template>

<script type="text/ecmascript-6">
import axios from 'axios';
const ERR_OK = 0;
 export default {
   props: {
     seller: {
       type: Object
     }
   },
   data () {
     return {
       goods: []
     };
   },
   mounted () {
     axios.get('/api/goods').then(result => {
       result = result.data;
       if (result.errno === ERR_OK) {
         this.goods = result.data;
       }
     });
   },
   components: {

   }
 };
</script>

<style scoped lang="stylus">

</style>
