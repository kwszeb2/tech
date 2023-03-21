<template>
<div class="wholeCard"> 
  <div class="card" v-for="img in imgs" :key="img.imgID">
    <div class="frontCard">
        <img :src="img.image" width="100" height="100">
        <div class="imgTitle">{{img.imgTitle}}</div>
    </div>
    <div class="frontButton">
       <button>More Info</button>
    </div>
  </div>
</div>
</template>

<script>

export default {
name: 'middleSection',
data() {
  return {
    imgs: [
      {
        imgTitle: "Finance",
        image: require('@/assets/images/finance.svg'),
        imgID: 2
      },
      {
        imgTitle: "Operations",
        image: require('@/assets/images/operations.svg'),
        imgID: 3
      },
      {
        imgTitle: "IT",
        image: require('@/assets/images/it.svg'),
        imgID: 4
      },
      {
        imgTitle: "Marketing",
        image: require('@/assets/images/marketing.svg'),
        imgID: 5
      },
      {
        imgTitle: "Services",
        image: require('@/assets/images/service.svg'),
        imgID: 6
      }
    ]
  }
} 
}

</script>

<style lang="sass" scoped>
$bg-color: #bde4f4
$secondary-color: #b1bed5

.wholeCard
  display: flex
  flex-direction: column
  @media (min-width: 768px) and (min-width: 1024px)
    display: flex
    flex-direction: row
    justify-content: space-evenly
    
.frontCard
  padding: 10px
  font-size: 20px
  @media (min-width: 768px) and (min-width: 1024px)
    padding: 40px
    font-size: 20px

.frontButton
  display: flex
  flex-direction: column
  @media (min-width: 768px) and (min-width: 1024px)
    display: flex
    flex-direction:column

button
  padding: 10px
  border-radius: 0 0 15px 15px 
  background-color: $bg-color
  font-size: 20px
  border: none
  @media (min-width: 768px) and (min-width: 1024px)
    padding: 10px
    border-radius: 0 0 15px 15px 
    background-color: $bg-color
    border: none
    &:hover
      background-color: $secondary-color

.card
  display: flex
  flex-direction: column
  border: 1px  solid black
  border-radius: 15px
  margin: 10px
  @media (min-width: 768px) and (min-width: 1024px)

.imgTitle
  color: black
  font-weight: bold
  padding-top: 15px

</style>