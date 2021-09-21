<template>
  <footer>
    <div class="fot-img">
      <div class="container">
        <div>
            <div>
                <ul>
                  <li><h3>DC COMICS</h3></li>
                  <li v-for="(link,index) in links[0].info" :key="index"><a href="">{{info.text}}</a></li>
                </ul>
              </div>
        </div>
        <div>
          <img src="@/assets/img/dc-logo-bg.png" alt="">
        </div>
      </div>
      <div>

      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
  data() {
    return {
      links : [
      {
          title: "DC COMICS",
          info: [
              {
              text: "characters",
              url: "#",
              },
              {
                  text: "comics",
                  url: "#",
              },
              {
                  text: "movie",
                  url: "#",
              },
              {
                  text: "TV",
                  url: "#",
              },
              {
                  text: "games",
                  url: "#",
              },
              {
                  text: "video",
                  url: "#",
              },
              {
                  text: "news",
                  url: "#",
              },
          ]
      },
      {
          title: "SHOP",
          info: [
              {
                  text: "Shop DC",
                  url: "#",
              },
              {
                  text: "Shop DC collectibles",
                  url: "#",
              },
          ]
      },
      {
          title: "DC",
          info: [
              {
              text: "Terms Of Use",
              url: "#",
              },
              {
                  text: "Privacy policy (New)",
                  url: "#",
              },
              {
                  text: "Ad Choices",
                  url: "#",
              },
              {
                  text: "Advertising",
                  url: "#",
              },
              {
                  text: "Jobs",
                  url: "#",
              },
              {
                  text: "Subscriptions",
                  url: "#",
              },
              {
                  text: "Talent Workshops",
                  url: "#",
              },
              {
                  text: "CPSC Certificates",
                  url: "#",
              },
              {
                  text: "Ratings",
                  url: "#",
              },
              {
                  text: "Shop Help",
                  url: "#",
              },
              {
                  text: "Contact Us",
                  url: "#",
              },
          ]
      },
      {
          title: "SITES",
          info: [
              {
              text: "DC",
              url: "#",
              },
              {
              text: "MAD Magazzine",
              url: "#",
              },
              {
              text: "DC Kids",
              url: "#",
              },
              {
              text: "DC Universe",
              url: "#",
              },
              {
              text: "DC Power Visa",
              url: "#",
              },
          ]
      },
  ]
  }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../style/Utilitis";
@import "../style/Footer";
</style>
