<template>
  <main>
    <div class="background-black">
      <div class="container font-s-50 pad-30">
        <span> -- Content goes hear -- </span>
      </div>
    </div>
    <div class="background-blu-light pad-50">
      <div class="container">
        <ul class="comics">
          <li v-for="(img,index) in imgs" :key="index">
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
export default {
  name: 'Main',
  data() {
    return {
      imgs : [
        {
          url : "buy-comics-digital-comics.png",
          title : "DIGITAL COMICS"
        },
        {
          url : "buy-comics-merchandise.png",
          title : "DC MERCHANDISE",
        },
        {
          url : "buy-comics-subcriptions.png",
          title : "SUBSCRIPTIONS",
        },
        {
          url : "buy-comics-shop-locator.png",
          title : "COMICS SHOP LOCATOR"
        },
        {
          url : "buy-dc-power-visa.svg",
          title : "DC POWER VISA",
        },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../style/Utilitis";
@import "../style/Main";

</style>
