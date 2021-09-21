<template>
  <main class="pos-rel z-index ">
    <div class="background-black">
      <div class="jumbotron">
          <img src="@/assets/img/jumbotron.jpg" alt="">
      </div>
      <div class="container pad-30">
        <div class="cdComicImg">
          <imgComic v-for="(img,index) in dcImgs" :key="index" :prod="img"/>
        </div>
        <div class="loadMore">
          <span>LOAD MORE</span>
        </div>
      </div>
    </div>
    <div class="background-blu-light pad-50">
      <div class="container">
        <ul class="comics">
          <li v-for="(img,index) in imgs" :key="index">
            <img :src="require(`@/assets/img/${img.url}`)" alt="">
            <div class="more">
              <span>{{img.title}}</span>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </main>
</template>

<script>
import imgComic from "@/components/ImgComics.vue";
import dcComics from "@/assets/data/dcComics.js";
import * as Img from '@/assets/data/Imgs.js';
export default {
  name: 'Main',
  components:{
    imgComic
  },
  dcComics,
  data() {
    return {
      imgs : Img.mainImg,
      dcImgs : dcComics,
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../style/Utilitis";
@import "../style/Main";
</style>
