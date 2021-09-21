<template>
  <header>
    <div class="container m-t-20">
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
export default {
  name: 'Header',
  data() {
    return {
          links : [
        {
          name : "CHARACTERS",
          url : "#",
          current : false,
        },
        {
          name : "COMICS",
          url : "#",
          current : true,
        },
        {
          name : "MOVIES",
          url : "#",
          current : false,
        },
        {
          name : "TV",
          url : "#",
          current : false,
        },
        {
          name : "GAMES",
          url : "#",
          current : false,
        },
        {
          name : "COLLECTIBLES",
          url : "#",
          current : false,
        },
        {
          name : "VIDEOS",
          url : "#",
          current : false,
        },
        {
          name : "FANS",
          url : "#",
          current : false,
        },
        {
          name : "NEWS",
          url : "#",
          current : false,
        },
        {
          name : "SHOP",
          url : "#",
          current : false,
        },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../style/Utilitis";
@import "../style/Header";
</style>
