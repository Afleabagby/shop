<template lang="pug">
  #home
    b-row
      b-col(cols="12" md="6" lg="3" v-for="(item, index) in items" :key="index")
        b-card(:title="item.name" :img-src="item.img" img-top :sub-title="'$'+item.price")
          b-button(variant="primary")
            font-awesome-icon(:icon="['fas', 'shopping-cart']")
            | &nbsp;加入購物車
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  data () {
    return {
      items: [
        {
          img: 'https://d.ecimg.tw/items/DJAD3JA900AXY5L/000001_1604889825.jpg',
          name: '賦權：當責式管理的延伸實踐（修訂版）(精裝)',
          price: 363
        },
        {
          img: 'https://d.ecimg.tw/items/DJAD3JA900AXWZR/000001_1603346056.jpg',
          name: '你的行為，決定你是誰：塑造企業文化最重要的事',
          price: 356
        },
        {
          img: 'https://d.ecimg.tw/items/DJAD3JA900AXQ1D/000001_1603180630.jpg',
          name: 'IG不NG從興趣出發創造幸福又賺錢的網紅雙贏人生',
          price: 356
        },
        {
          img: 'https://d.ecimg.tw/items/DJAD3JA900AXWZM/000001_1603346147.jpg',
          name: '與成功有約：高效能人士的七個習慣（30週年全新增訂版）',
          price: 435
        }
      ]
    }
  }
}
</script>
