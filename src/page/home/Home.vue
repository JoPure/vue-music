<template>
  <div id="my_music">
    <div class="typelist">
      <i class="info icon-music">
        {{mymusic_1}}
      </i>
      <div class="typelist-detail">
         <span class="name">我的音乐</span>
         <span class="count">(28)</span>
      </div>
    </div>
    </div>
</template>
<script type="text/ecmascript-6">
  import axios from 'axios'
  import {mapState} from 'vuex'
  export default {
    data() {
      return {
        mymusic_1:'我的音乐'
      }
    },
    mounted() {
      this.$nextTick(() => {
      })
    },
    methods: {},
    filters: {},
    computed: {
      ...mapState([])
    }
  }
</script>
<style lang="scss" type="text/scss">
    @import '../../assets/css/base';

  .typelist{
    margin-top: pr(25);
    height: pr(20);
    position: relative;
    background: rgb(247, 247, 247);
  .typelist-detail{
      height: 100%;
      line-height: pr(50);
      margin-left: pr(50);
      box-sizing: border-box;
      font-size: 0;
  .count{
    color: #aaa;
    font-size: pr(10);
    font-weight: 400;
    vertical-align: middle;
    }
  }
}
</style>
