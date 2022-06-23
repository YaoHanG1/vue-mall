<template>
  <div>
    <h2>分类</h2>
    <div class="wrapper">
      <ul class="connor"> 
      <button @click="btnClick">按钮</button>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
      <li>一打</li>
    </ul>
    </div>
  </div>
</template>

<script>
import BScroll from 'better-scroll'
export default {
  name: 'Category',
  data() {
    return {
      scroll: null
    }
  },
  mounted() {
    this.scroll = new BScroll(document.querySelector('.wrapper'),{
      probeType: 3,
      pullUpLoad: true
    })

    this.scroll.on('scroll', (position) => {
      // console.log(position);
    })

    this.scroll.on('pullingUp', () => {
      console.log('上啦加载更多');
    })
  },
  methods: {
    btnClick() {
      console.log('btnclick');
    }
  }
}

</script>

<style scoped>
  .wrapper {
    height: 150px;
    /* overflow-y: scroll; */
    overflow: hidden;
  }
</style>