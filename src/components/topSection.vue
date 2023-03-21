<template>
  <div class="wholePage">
    <div class="topnav">
      <div id="myLinks">
        <a href="">News</a>
        <a href="">Contact</a>
        <a href="">About</a>
      </div>
      <!-- "Hamburger menu" / "Bar icon" to toggle the navigation links -->
      <div v-on:click="myFunction">
        <img :src="('https://img.icons8.com/external-tal-revivo-bold-tal-revivo/24/null/external-horizontal-separated-bars-representing-hamburger-menu-layout-grid-bold-tal-revivo.png')" class="icon">
      </div>
    </div>
    <div class="heroBanner">
      <img :src="require('@/assets/images/office.jpg')">
    </div>
    <div class="paraContent">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur quis orci nec diam maximus feugiat at eget enim. Suspendisse et tortor vitae risus aliquam dignissim. Vivamus eleifend orci ac nisi fringilla egestas. Integer hendrerit massa a elit suscipit blandit at luctus arcu. Curabitur vel nulla pulvinar, placerat elit ac, dictum erat. Aliquam ligula velit, imperdiet ac purus quis, auctor eleifend nibh. Duis a rhoncus neque. Suspendisse ac diam sit amet ipsum feugiat semper a sed libero. Praesent semper lacinia ligula in facilisis. In tortor risus, blandit eu dictum nec, pulvinar a mi.
      </p>
      <p>
        Nullam volutpat elit sed felis volutpat congue. Maecenas eu sem convallis, tincidunt tortor eget, vestibulum est. Aliquam convallis erat vel est sodales molestie. Pellentesque at mollis tortor. Suspendisse non venenatis magna. Morbi neque ante, pharetra eget elit nec, viverra fringilla nisl. Praesent vitae ante sed tortor volutpat pharetra lobortis maximus est. Curabitur congue ac ante nec faucibus. Sed rutrum lectus enim, id malesuada lacus dapibus nec. Suspendisse viverra lectus sed faucibus fringilla.
      </p>
      <p>
        Donec pharetra metus sed mi rutrum posuere. Proin a scelerisque odio. Mauris lobortis, leo at congue auctor, magna dui gravida ante, sodales cursus lorem augue et dolor. Phasellus nec aliquet risus. Quisque volutpat at nunc et imperdiet. Quisque porttitor turpis ac sem consequat, sit amet vehicula ante consectetur. Integer at vehicula nunc, et hendrerit sem. Pellentesque tincidunt, urna cursus gravida tempus, nisl massa vulputate ligula, sed pellentesque nunc neque tempus purus. Suspendisse tempus sagittis magna non tincidunt. Cras vestibulum finibus arcu vel commodo. In sit amet volutpat ex. Aliquam pretium, ex ac pulvinar cursus, risus libero porttitor nisl, in sollicitudin massa nunc ac nisl.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'topSection',
  methods: {
    myFunction() {
      var x = document.getElementById("myLinks");
      if (x.style.display === "block") {
        x.style.display = "none";
      } else {
        x.style.display = "block";
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>


.topnav
  overflow: hidden
  background-color: black
  position: relative
  color: white
  padding: 24px
  text-decoration: none
  font-size: 17px
  display: block
  @media (min-width: 768px) and (min-width: 1024px)
    overflow: visible
  #myLinks
    display: none
    @media (min-width: 768px) and (min-width: 1024px)
      display: flex
      justify-content: space-evenly
  a
    color: white
    padding: 14px 16px
    text-decoration: none
    font-size: 17px
    display: block
    @media (min-width: 768px) and (min-width: 1024px)
      display: inline
      &:hover
        color: black
        background-color: white

.icon
    width: 24px !important
    height: 24px !important
    display: block
    position: absolute
    left: 10px
    top: 10px
    background-color: white
    @media (min-width: 768px) and (min-width: 1024px)
      display: none

img
  background-size: cover
  width: 100%
  height: auto
  @media (min-width: 768px) and (min-width: 1024px)
    background-size: cover
    width: 100%
    height: auto

p
  display: flex
  flex-direction: column
  flex-wrap: wrap
  text-align: justify
  @media (min-width: 768px) and (min-width: 1024px)
     text-align: justify
  

</style>
