<template>
  <main class="pos-rel z-index ">
    <div class="background-black">
      <div class="container font-s-50 pad-30">
        <span> -- Content goes hear -- </span>
      </div>
    </div>
    <div class="background-blu-light pad-50">
      <div class="container">
        <ul class="comics">
          <li v-for="(img,index) in imgs" :key="index">
            <img :src="require(`@/assets/img/${img.url}`)" alt="">
            <div>
              <span>{{img.title}}</span>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </main>
</template>

<script>
import * as Img from '@/assets/data/Imgs.js'
export default {
  name: 'Main',
  data() {
    return {
      imgs : Img.mainImg
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../style/Utilitis";
@import "../style/Main";

</style>
