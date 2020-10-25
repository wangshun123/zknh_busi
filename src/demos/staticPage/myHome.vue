<template>

  <div>
    <div class="note" :style ="note"></div>
      <p><spen id="test-content">准康云线上平台</spen></p>
    <grid :show-lr-borders="false" :show-vertical-dividers="false">
      <grid-item link="/component/cell" :label="$t('Go to Cell')">
        <img slot="icon" src="../../assets/grid_icon.png">
      </grid-item>
      <grid-item :link="{ path: '/component/cell'}" :label="$t('Go to Cell')">
        <img slot="icon" src="../../assets/grid_icon.png">
      </grid-item>
      <grid-item link="/component/cell" @on-item-click="onItemClick">
        <img slot="icon" src="../../assets/grid_icon.png">
        <span slot="label">{{ $t('Go to Cell') }}</span>
      </grid-item>
      <grid-item link="/component/cell" @on-item-click="onItemClick">
        <img slot="icon" src="../../assets/grid_icon.png">
        <span slot="label">{{ $t('Go to Cell') }}</span>
      </grid-item>
    </grid>
    <grid :show-lr-borders="false" :show-vertical-dividers="false">
      <grid-item link="/component/cell" :label="$t('Go to Cell')">
        <img slot="icon" src="../../assets/grid_icon.png">
      </grid-item>
      <grid-item :link="{ path: '/component/cell'}" :label="$t('Go to Cell')">
        <img slot="icon" src="../../assets/grid_icon.png">
      </grid-item>
      <grid-item link="/component/cell" @on-item-click="onItemClick">
        <img slot="icon" src="../../assets/grid_icon.png">
        <span slot="label">{{ $t('Go to Cell') }}</span>
      </grid-item>
      <grid-item link="/component/cell" @on-item-click="onItemClick">
        <img slot="icon" src="../../assets/grid_icon.png">
        <span slot="label">{{ $t('Go to Cell') }}</span>
      </grid-item>
    </grid>
  </div>



</template>

<i18n>
Grid:
Go to Cell:
zh-CN:准康商城

</i18n>

<script>
import { Grid, GridItem, GroupTitle } from 'vux'

export default {
  name: 'productdetailspage',
  data () {
    return {
      note: {
        backgroundImage: 'url(' + require('../../assets/logo_520.png') + ')',
        backgroundRepeat: 'no-repeat',
        backgroundSize: '25px auto',
        marginTop: '5px'
      }
    }
  },
  components: {
    Grid,
    GridItem,
    GroupTitle

  },
  methods: {
    onItemClick () {
      console.log('on item click')
    }
  }
}
</script>

<style scoped>

#test-content {
  display:block;
  margin:0 auto;
  width:140px;
  height: 100px;
  text-align: center;
  line-height:100px;
  font-size:20px;
  color: #00000c;
  font-style:italic;
}
.note{
  background:url("../../assets/logo_520.png");
}
</style>
