<template>
  <div class="img-comics">
    <img :src="prod.thumb" alt="">
    <p>{{prod.series}}</p>
  </div>
</template>

<script>
export default {
    props: ["prod"],
}
</script>

<style>
 .img-comics  img {
                width: 90%;
                height: 25vh;
                object-fit: cover;
                object-position: top;
        } 
</style>