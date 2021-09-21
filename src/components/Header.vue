<template>
  <header>
    <div class="container d-felx m-t-20">
      <div class="logo">
        <img src="@/assets/img/dc-logo.png" alt="">
      </div>
      <div class="menu">
        <ul>
          <li v-for="(link,index) in links" :key="index" :class="(link.current === true) ? 'active': null">
            <a :href="link.url">{{link.name}}</a>
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>

<script>
import * as Links from "@/assets/data/Links.js"
export default {
  name: 'Header',
  data() {
    return {
          links : Links.headerLinks
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../style/Utilitis";
@import "../style/Header";
</style>
