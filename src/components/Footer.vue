<template>
  <footer>
    <div class="fot-img">
      <div class="container-fot">
        <div class="foot">
            <div>
                <ul>
                  <li><h3>DC COMICS</h3></li>
                  <li v-for="(link,index) in links[0].info" :key="index"><a href="">{{link.text}}</a></li>
                </ul>
                 <ul class="pad-top">
                  <li><h3>SHOP</h3></li>
                  <li v-for="(link,index) in links[1].info" :key="index"><a href="">{{link.text}}</a></li>
                </ul>
            </div>
            <div>
                 <ul>
                  <li><h3>DC</h3></li>
                  <li v-for="(link,index) in links[2].info" :key="index"><a href="">{{link.text}}</a></li>
                </ul>
            </div>
            <div>
                 <ul>
                  <li><h3>SITES</h3></li>
                  <li v-for="(link,index) in links[3].info" :key="index"><a href="">{{link.text}}</a></li>
                </ul>
            </div>
        </div>
        <div>
          <img src="@/assets/img/dc-logo-bg.png" alt="">
        </div>
      </div>
    </div>
     <div class="background-black pos-rel" >
       <div class="container-fot-2 d-felx align-center">
          <div class="container-fot-1 pad-50">
              <div class="sing">
                  <h2>SING UP NOW</h2>
              </div>
          </div>
          <div class="social">
              <h2 class="follow">FOLLOW US</h2>
              <ul>
                  <li v-for="(Img,index) in Imgs" :key="index"><img :src="require(`@/assets/img/${Img.info}`)" alt=""></li>
              </ul>
          </div>
        </div>
      </div>
  </footer>
</template>

<script>
import * as Links from "@/assets/data/Links.js";
import * as Img from '@/assets/data/Imgs.js'
export default {
  name: 'Footer',
  data() {
    return {
      links : Links.footerLinks,
      Imgs : Img.footerSocials
  }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../style/Utilitis";
@import "../style/Footer";
@import "../style/Main";
</style>
