<template>
  <div class="rkhy-tabbar" :class="{
      'is-fixed': fixed
    }">
    <slot></slot>
  </div>
</template>

<script>
    /**
     * @param {Boolean} fixed - 是否固定
     *
     * 此组件需要和tab-con,tab-con-item,tab-item一起使用，例：
     *
     <rkhy-tabbar v-model="selected">
     <rkhy-tabitem id="testest1">111111</rkhy-tabitem>
     <rkhy-tabitem id="testest2">22222</rkhy-tabitem>
     <rkhy-tabitem id="testest3">333333</rkhy-tabitem>
     </rkhy-tabbar>
     <rkhy-tabcon v-model="selected" :swipeable="true">
     <rkhy-tabconitem  :sid="'testest1'">
     sdfsdfsdf1
     </rkhy-tabconitem>
     <rkhy-tabconitem  :sid="'testest2'">
     sdfsdfsd2
     </rkhy-tabconitem>
     <rkhy-tabconitem  :sid="'testest3'">
     sdfsdfsd3
     </rkhy-tabconitem>
     </rkhy-tabcon>
     **/
export default {
  name: 'RkhyTabbar',

  props: {
    fixed: Boolean,
    value: {},
  },
  created(){
      //console.log(this.value)
  }
};
</script>
