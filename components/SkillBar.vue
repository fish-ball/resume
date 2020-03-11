<template>
  <ul class="bar" :class="'level-'+level">
    <li>
      <template v-if="level==='c'">了解</template>
    </li>
    <li>
      <template v-if="level==='b'">掌握</template>
    </li>
    <li>
      <template v-if="level==='a'">熟练</template>
    </li>
  </ul>
</template>

<script>
export default {
  props: {
    level: { type: String }
  }
}
</script>

<style lang="less" scoped>
@import '../libs/less-template/colors';

ul.bar {
  font-size: 12px;
  vertical-align: middle;
  text-align: center;
  display: inline-block;
  margin-left: 1em;
  li {
    padding: 0 4px;
    height: 16px;
    line-height: 16px;
    float: left;
    margin-left: -1px;
    border-left: 1px solid white;
    /*border: 1px solid #CCC;*/
    color: white !important;
    &:first-of-type {
      border-radius: 4px 0 0 4px;
      border: 0;
    }
    &:last-of-type {
      border-radius: 0 4px 4px 0;
    }
  }
  &.level-a {
    li {
      background: @color-red-accent-2;
    }
  }
  &.level-b {
    li {
      background: @color-orange;
    }
  }
  &.level-c {
    li {
      background: @color-yellow-darken-1;
    }
  }
}
</style>
